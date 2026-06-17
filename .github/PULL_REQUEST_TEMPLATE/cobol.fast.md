# Revue de code rapide de COBOL

## Général
- [ ] Code lisible et bien structuré																		
- [ ] Pas de duplication de code																		
- [ ] Valider que la requête SQL est bien conforme aux spécifications du requis. Requêtes SQL paramétrées																		
- [ ] Si des curseurs sont utilisés s'assurer qu'ils sont biens fermés																		

## Normes et lisibilité
- [ ] Aucune variable, procédure, section ou CopyBook inutile n’est présent																		
- [ ] La numérotation des procedure est cohérente et conforme aux normes																		
- [ ] Les structures conditionnelles sont simples et lisibles																		
- [ ] S'assurer que chaque instruction PERFORM est bien délimitée par une instruction THRU correspondante																		
- [ ] S'assurer que les variables utilisées ont la bonne taille pour le nombre de chiffres [PIC(9)] ou de caractères [PIC(X)] asignés																		
- [ ] Le code modifié ne génère pas de nouveau message d'avertissement (Warning). 																		
- [ ] Valider le point '.' à la fin d'une instruction pour s'assurer que l'exécution est celle souhaitée.																		
