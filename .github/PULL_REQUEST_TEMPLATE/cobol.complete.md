# Revue de code complète de COBOL

## Général

- [ ] Éliminer le code mort ou inutilisé - Si le dev travail dessus et tombe sur du code mort oui ok de le retirer
- [ ] Code lisible et bien structuré
- [ ] Pas de duplication de code
- [ ] Valider que la requête SQL est bien conforme aux spécifications du requis. Requêtes SQL paramétrées
- [ ] Les requêtes doivent toujours être paramétrées (si variables) ou utiliser une Stored Proc.
- [ ] Si des curseurs sont utilisés s'assurer qu'ils sont biens fermés
- [ ] Retourner seulement les colonnes et rangées nécessaires
- [ ] Aucun `SELECT  *`
- [ ] Valider les données en entrée (fichiers, paramètres batch)
- [ ] Les noms des variables respectent la nomenclature dans le programme courant
- [ ] Aucune variable, procédure, section ou CopyBook inutile n’est présent
- [ ] Le nom des procédures est significatif
- [ ] La numérotation des procedure est cohérente et conforme aux normes
- [ ] Tous les fichiers à ouvrir l'ont été selon le bon mode (INPUT, I-O ou OUTPUT)
- [ ] Le FILESTATUS est vérifié pour les énoncés entrées et de sorties (OPEN, READ, WRITE, CLOSE...)
- [ ] Les instructions sont utilisées de manière appropriée et optimisée (EVALUATE, ADD, COMPUTE…)
- [ ] Les structures conditionnelles sont simples et lisibles
- [ ] S'assurer que chaque instruction PERFORM est bien délimitée par une instruction THRU correspondante
- [ ] Ne pas ajouté inutilement de STOP RUN ou GOBACK pour un même programme
- [ ] S'assurer que les variables utilisées ont la bonne taille pour le nombre de chiffres [PIC(9)] ou de caractères [PIC(X)] asignés
- [ ] Le débordement de table est vérifié
- [ ] Les niveaux 88 sont utilisés lorsqu'ils existent
- [ ] Le code modifié ne génère pas de nouveau message d'avertissement (Warning).
- [ ] Valider le point '.' à la fin d'une instruction pour s'assurer que l'exécution est celle souhaitée.
