# Club robotique

Espace commun pour suivre les projets, la compta et les ressources du club robotique.

## Actions rapides

Les boutons demandent le nom de la note, la créent dans le bon dossier, puis appliquent le bon template.

> [!tip] Projets
> `button-projet-perso` `button-projet-groupe` `button-projet-fil-rouge`

> [!success] Compta
> `button-depense`

> [!info] Ressources / doc
> `button-ressource-video` `button-ressource-docs` `button-ressource-livre` `button-ressource-forum`

## Vue d'ensemble

![[Tableau de bord.base#Projets]]

## Compta

- [[COMPTA/Livret de compte|Livret de compte]]
- Créer une dépense dans `COMPTA/dépenses/` avec le bouton dédié ou le modèle [[_templates/dépense|Dépense]].

![[Tableau de bord.base#Compta]]

## Ressources / doc

Ajouter les ressources dans `RESSOURCE/video`, `RESSOURCE/docs`, `RESSOURCE/livre` ou `RESSOURCE/forum` avec les boutons dédiés.

![[Tableau de bord.base#Ressources]]

## Ajouter une entrée

1. Cliquer sur le bouton correspondant.
2. Donner un nom clair à la note.
3. Remplir les propriétés restantes en haut de la note : les bases se mettent à jour automatiquement.

## Dossiers

- `PROJETS/perso` : projets portés par une personne.
- `PROJETS/groupe` : projets d'équipe.
- `PROJETS/fil rouge` : gros projets structurants du club.
- `COMPTA/dépenses` : une note par dépense.
- `RESSOURCE/*` : vidéos, docs, livres, forums.

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
