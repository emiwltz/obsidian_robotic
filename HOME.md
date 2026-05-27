---
cssclass: club-home
cssclasses:
  - club-home
---
# 🤖 Club robotique

| 🎛️ Centre de contrôle                                                                                                                                                                                                                                                                                              | 🚦 Mode d'emploi                                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Dashboard unique pour **créer**, **suivre** et **retrouver** rapidement tout ce qui fait vivre le club : projets, compta, ressources et documentation.<br><br>**Accès rapide** · [[#⚡ Actions rapides]] · [[#📊 Vue d'ensemble]] · [[#🗂️ Carte du vault]] · [[COMPTA/Livret de compte]] · [[Tableau de bord.base]] | 1. Cliquer sur une action.<br>2. Nommer clairement la note.<br>3. Remplir les propriétés.<br>4. Les vues se mettent à jour. |

---

## ⚡ Actions rapides

| 🛠️ Projets                                                                                                                                         | 💶 Compta                                                                                                                                                |
| --------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Créer une idée perso, un projet d'équipe ou un fil rouge structurant.<br><br>`button-projet-perso` `button-projet-groupe` `button-projet-fil-rouge` | Ajouter une dépense, une entrée d'argent ou ouvrir le suivi financier.<br><br>`button-depense` `button-entree-argent`<br><br>[[COMPTA/Livret de compte]] |

| 📚 Ressources | 🧭 Accès utiles |
|---|---|
| Archiver une vidéo, une documentation, un livre/PDF ou un post de forum.<br><br>`button-ressource-video` `button-ressource-docs` `button-ressource-livre` `button-ressource-forum` | Aller directement aux pages qui servent le plus pendant une séance.<br><br>[[Tableau de bord.base]] · [[COMPTA/Livret de compte]] · [[README]]<br><br>[[_templates/Projet]] · [[_templates/Ressource]] |

---

## 🧭 Navigation claire

| 🛠️ Projets | 💶 Compta | 📚 Ressources | 🧩 Templates |
|---|---|---|---|
| Idées, prototypes, projets d'équipe, fil rouge.<br><br>Priorité : `statut`, `responsable`, `priorite`, `echeance`.<br><br>[[#🛠️ Suivi projets]] | Dépenses, entrées, justificatifs.<br><br>Priorité : `date`, `montant`, `statut`, `categorie`, `projet`.<br><br>[[#💶 Suivi compta]] | Vidéos, docs, livres/PDF, forums.<br><br>Priorité : `sujet`, `lien`, `niveau`, `statut`.<br><br>[[#📚 Ressources partagées]] | Modèles utilisés par les boutons.<br><br>À modifier seulement si la structure change.<br><br>[[_templates/Projet]] · [[_templates/Ressource]] |

---

## 📊 Vue d'ensemble

Les vues ci-dessous viennent de [[Tableau de bord.base]] et se mettent à jour automatiquement avec les notes de `PROJETS/`, `COMPTA/` et `RESSOURCE/`.

### 🛠️ Suivi projets

![[Tableau de bord.base#Projets]]

### 💶 Suivi compta

![[Tableau de bord.base#Compta]]

### 📚 Ressources partagées

![[Tableau de bord.base#Ressources]]

---

## 🗂️ Carte du vault

| 🛠️ `PROJETS/` | 💶 `COMPTA/` |
|---|---|
| `perso/` · projets portés par une personne<br>`groupe/` · projets d'équipe<br>`fil rouge/` · gros projets structurants | `dépenses/` · sorties d'argent<br>`entrées/` · entrées d'argent<br>[[COMPTA/Livret de compte]] · synthèse financière |

| 📚 `RESSOURCE/` | 🧩 `_templates/` |
|---|---|
| `video/` · vidéos utiles<br>`docs/` · documentation technique<br>`livre/` · livres, PDF, références longues<br>`forum/` · posts et discussions utiles | Modèles appliqués automatiquement par les boutons.<br>À modifier uniquement quand les propriétés ou dossiers changent. |

---

## ✅ Rituel rapide du club

| Pendant la séance | Après la séance |
|---|---|
| ☐ Ajouter les nouvelles idées / nouveaux projets.<br>☐ Mettre à jour les statuts des projets actifs.<br>☐ Saisir les dépenses et entrées récentes. | ☐ Joindre ou lier les justificatifs manquants.<br>☐ Classer les ressources utiles trouvées.<br>☐ Relier ressources et compta au projet concerné. |

## 🏷️ Repères de statuts

| 🛠️ Projets | 💶 Dépenses | 💰 Entrées | 📚 Ressources |
|---|---|---|---|
| `idee` · `en-cours` · `bloque` · `termine`<br>Où en est le projet ? | `a-rembourser` · `rembourse` · `valide`<br>Faut-il encore agir ? | `a-encaisser` · `encaisse` · `valide`<br>L'argent est-il bien arrivé ? | `a-voir` · `utile` · `archive`<br>La ressource sert-elle encore ? |

---

<!-- Définitions Buttons masquées en rendu. -->

```button
name 🤖 Projet perso
type note(PROJETS/perso/Projet perso, tab) template
action Projet - perso
prompt true
class club-button club-button-projets
color blue
width 12
height 2.4
align center middle
hidden true
```
^button-projet-perso

```button
name 👥 Projet groupe
type note(PROJETS/groupe/Projet groupe, tab) template
action Projet - groupe
prompt true
class club-button club-button-projets
color blue
width 12
height 2.4
align center middle
hidden true
```
^button-projet-groupe

```button
name 🚩 Fil rouge
type note(PROJETS/fil rouge/Projet fil rouge, tab) template
action Projet - fil rouge
prompt true
class club-button club-button-projets
color blue
width 12
height 2.4
align center middle
hidden true
```
^button-projet-fil-rouge

```button
name 💶 Dépense
type note(COMPTA/dépenses/Dépense, tab) template
action dépense
prompt true
class club-button club-button-compta
color green
width 12
height 2.4
align center middle
hidden true
```
^button-depense

```button
name 💰 Entrée d'argent
type note(COMPTA/entrées/Entrée argent, tab) template
action entrée d'argent
prompt true
class club-button club-button-compta-in
color green
width 14
height 2.4
align center middle
hidden true
```
^button-entree-argent

```button
name 🎬 Vidéo
type note(RESSOURCE/video/Ressource video, tab) template
action Ressource - video
prompt true
class club-button club-button-ressources
color purple
width 9
height 2.4
align center middle
hidden true
```
^button-ressource-video

```button
name 📄 Doc
type note(RESSOURCE/docs/Ressource docs, tab) template
action Ressource - docs
prompt true
class club-button club-button-ressources
color purple
width 9
height 2.4
align center middle
hidden true
```
^button-ressource-docs

```button
name 📚 Livre
type note(RESSOURCE/livre/Ressource livre, tab) template
action Ressource - livre
prompt true
class club-button club-button-ressources
color purple
width 9
height 2.4
align center middle
hidden true
```
^button-ressource-livre

```button
name 💬 Forum
type note(RESSOURCE/forum/Ressource forum, tab) template
action Ressource - forum
prompt true
class club-button club-button-ressources
color purple
width 9
height 2.4
align center middle
hidden true
```
^button-ressource-forum
