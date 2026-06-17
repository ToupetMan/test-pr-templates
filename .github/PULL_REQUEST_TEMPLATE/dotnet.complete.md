# Revue de code .NET

## Général
- [ ] Éliminer le code inutilisé - S'il a été écrit dans le cadre du travail en cours
- [ ] Éviter Microsoft.VisualBasic si non requis                           
- [ ] Un contrat doit être totalement indépendant
- [ ] Code et Méthode lisible et bien structuré
- [ ] Utiliser les régions seulement si pertinent

## Structure
- [ ] Une méthode a une seule responsabilité, ne pas être trop complexe
- [ ] Séparation des couches (UI, logique, données)
- [ ] Pas de duplication de code
- [ ] Utiliser l'héritage lorsque nécessaire
- [ ] Classes avec responsabilité claire

## SQL et fichiers
- [ ] Valider que la requête SQL est bien conforme aux spécifications du requis. Requêtes SQL paramétrées  (aucun concat SQL)
- [ ] Les requêtes doivent toujours être paramétrées (si variables) ou utiliser une Stored Proc.
- [ ] Une nouvelle Stored Proc ne devrait pas faire de logique d'affaires
- [ ] Le type Exact et la longueur des paramètres doivent toujours être indiqués dans les clauses WHERE lorsque la colonne n'est pas une clé primaire. Pour éviter les transtypages empêchant l'utilisation des index.
- [ ] Utiliser Using pour libérer les ressources le plus rapidement possible(connexion, Readers, Handle,, …), en .NET
- [ ] Retourner seulement les colonnes et rangées nécessaires
- [ ] Pas de `SELECT *`
- [ ] Pas d'appel BD dans une boucle
- [ ] Arrimer les modifications du fichier de configuration avec les fichiers de configuration des autres environnements
- [ ] Libérer correctement les connexions BD

## Exceptions et erreurs
- [ ] Pas de `On Error Resume Next`
- [ ] Pas de `Catch` vide
- [ ] Pas de logique métier dans les `Try/Catch`
- [ ] Exceptions non masquées (remontées ou traitées correctement)

## Performance
- [ ] Pas de recalcul inutile en boucle
- [ ] Emmagasiner la valeur d'une propriété dans une variable si cette propriété est utilisée plus d'une fois.
- [ ] Pas d’appel BD inutile
- [ ] Ne jamais utiliser Try / Catch pour implanter une logique de traitement. Réserver les exceptions au traitement des erreurs exclusivement
- [ ] Tester les requêtes BD si impact sur la performance
- [ ] Vérifier que la performance répond aux critères du projet.
- [ ] Utiliser DirectCast lorsque possible.

## Sécurité
- [ ] Validation des entrées utilisateur
- [ ] Aucune donnée sensible exposée
