# 🤖 Vault du club robotique

> [!summary] Objectif
> Ce vault Obsidian sert de base commune pour suivre les **projets**, la **compta**, les **ressources** et la documentation du club.

## 🚀 Démarrer rapidement

| Besoin | Où aller |
|---|---|
| Créer une nouvelle entrée | [[HOME]] |
| Voir les tableaux dynamiques | [[Tableau de bord.base]] |
| Suivre la compta | [[Livret de compte]] |

> [!tip] Workflow conseillé
> 1. Ouvrir [[HOME]].  
> 2. Cliquer sur le bouton adapté : projet, dépense, entrée d'argent ou ressource.  
> 3. Donner un nom clair à la note.  
> 4. Compléter les propriétés en haut de la note.  
> Les vues se mettent ensuite à jour automatiquement.

## 🗂️ Organisation du vault

```text
PROJETS/
  perso/        projets portés par une personne
  groupe/       projets d'équipe
  fil rouge/    projets structurants du club

COMPTA/
  dépenses/     sorties d'argent
  entrées/      entrées d'argent

RESSOURCE/
  video/        vidéos utiles
  docs/         documentation technique
  livre/        livres, PDF, références longues
  forum/        posts et discussions utiles

_templates/     modèles utilisés par les boutons
```

## ✍️ Créer une note

### 🛠️ Projets

| Type | Dossier | À remplir en priorité |
|---|---|---|
| Projet perso | `PROJETS/perso/` | `statut`, `responsable`, `priorite`, `echeance` |
| Projet groupe | `PROJETS/groupe/` | `statut`, `responsable`, `participants`, `priorite` |
| Fil rouge | `PROJETS/fil rouge/` | `statut`, `responsable`, `participants`, `echeance` |

### 💶 Compta

| Type | Dossier | Propriétés importantes |
|---|---|---|
| Dépense | `COMPTA/dépenses/` | `date`, `montant`, `payeur`, `statut`, `categorie`, `projet` |
| Entrée d'argent | `COMPTA/entrées/` | `date`, `montant`, `source`, `recu_par`, `moyen`, `statut` |

> [!important] Justificatifs
> Ajouter les factures, tickets ou preuves de paiement en pièce jointe, puis les lier dans la propriété `justificatif`.

### 📚 Ressources

| Type | Dossier | À remplir en priorité |
|---|---|---|
| Vidéo | `RESSOURCE/video/` | `sujet`, `lien`, `niveau`, `statut` |
| Doc | `RESSOURCE/docs/` | `sujet`, `lien`, `niveau`, `statut` |
| Livre | `RESSOURCE/livre/` | `sujet`, `lien`, `niveau`, `statut` |
| Forum | `RESSOURCE/forum/` | `sujet`, `lien`, `niveau`, `statut` |

## 📊 Tableaux de bord

Le fichier [[Tableau de bord.base]] regroupe les vues principales :

| Vue | Contenu |
|---|---|
| **Projets** | suivi des projets du club |
| **Compta** | dépenses + entrées d'argent avec solde signé |
| **Dépenses** | vue dédiée aux sorties d'argent |
| **Entrées** | vue dédiée aux rentrées d'argent |
| **Ressources** | ressources et documentation partagées |

## ✅ Bonnes pratiques

- Une note = une entrée claire : un projet, une dépense, une entrée d'argent ou une ressource.
- Utiliser des noms explicites : `Achat servos MG996R`, `Projet bras robotique`, etc.
- Lier les dépenses et ressources à un projet quand c'est pertinent avec `projet`.
- Garder les templates dans `_templates/` simples et propres.
- Faire des commits Git réguliers après les grosses modifications.

## 🔌 Plugins utilisés

| Plugin | Usage |
|---|---|
| **Bases** | tableaux dynamiques |
| **Buttons** | boutons de création rapide sur [[HOME]] |
| **Templates** | modèles de notes dans `_templates/` |
| **Git** | versionner et synchroniser le vault |
| **Excalidraw** | schémas, croquis mécaniques/électroniques |
