# Introduction 3D pour un site - Ouverture d'un ordinateur portable

Une entrée pour un site web réutilisable : un ordinateur portable s'ouvre, la caméra
plonge vers son écran, et le site apparaît sur ce dernier (occupant tout l'espace et supprimant la scène 3d une fois le site affiché).  
Il suffit de déposer son propre site dans le dossier prévu, sans toucher au reste.

**Auteur :** Rafaël HOCQUEL
**Version :** 0.5 - en construction

## Le principe

| Étape | Ce qui se passe |
|-------|-----------------|
| 1 | La scène s'ouvre sur un ordinateur portable |
| 2 | Son capot se lève, l'écran s'allume |
| 3 | La caméra avance vers l'écran |
| 4 | L'écran passe au premier plan et le site apparaît, à sa taille normale |
| 5 | Le visiteur se retrouve simplement sur le site, avec sa navigation habituelle |

L'introduction ne se joue qu'une fois, et reste facultative : un lien direct
vers le site doit toujours être possible, pour les visiteurs pressés comme pour
les moteurs de recherche.

## Comment l'utiliser

| Ce que vous voulez changer | Où |
|---------------------------|-----|
| **Votre site** | Dans le dossier prévu à cet effet : ses fichiers y sont servis tels quels |
| Le titre et la description | `app/layout.tsx` |
| Les couleurs | `app/globals.css`, où la palette est définie en variables |
| La police | `app/fonts`, en la déposant dans le dépôt plutôt qu'en la demandant à un service externe |
| Le logo et la signature | `public/logos` et `public/signatures`, qui contiennent ici des exemples à remplacer |

Rien d'autre n'est à modifier : la durée de l'ouverture, l'angle de la caméra et
le style de la scène sont regroupés au même endroit dans le code de
l'introduction.

## Où en est le projet

| Étape | État |
|-------|------|
| Socle Next.js, TypeScript et Tailwind | Fait |
| Police Source Serif 4 hébergée localement | Fait |
| Palette de couleurs en variables | Fait |
| Titre et description du site | Fait |
| Scène 3D : l'ordinateur et son ouverture | Fait |
| Transition vers le site déposé | À venir |
| Version allégée pour les téléphones | À venir |


## Technos

| Outil | Rôle |
|-------|------|
| **Next.js 16** | Structure du projet et service des fichiers |
| **React 19** | Composants |
| **TypeScript** | Typage |
| **Tailwind CSS 4** | Styles, avec la palette en variables |
| **ESLint** | Vérification du code |

## Lancer le projet

```bash
git clone https://github.com/rafael-hocquel/3d-laptop-website-intro.git
cd 3d-laptop-website-intro
npm install
npm run dev
