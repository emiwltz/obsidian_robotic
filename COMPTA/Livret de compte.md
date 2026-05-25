# Livret de compte

Une ligne de compta = une note :

- dépense : `COMPTA/dépenses/`, modèle [[_templates/dépense|Dépense]] ;
- entrée d'argent : `COMPTA/entrées/`, modèle [[_templates/entrée d'argent|Entrée d'argent]].

![[Tableau de bord.base#Compta]]

## Règles simples

- Toujours remplir `date`, `montant`, `statut` et `categorie`.
- Lier l'entrée au projet concerné si possible (`projet: lien vers la note du projet`).
- Pour une dépense, remplir `payeur`.
- Pour une entrée d'argent, remplir `source`, `recu_par` et `moyen` si possible.
- Mettre la photo / facture / justificatif en pièce jointe et la lier dans `justificatif`.
