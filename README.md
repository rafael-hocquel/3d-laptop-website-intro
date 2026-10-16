# Socle d'une introduction 3D pour un site - Ouverture d'un ordinateur portable

Ce dépôt est le **socle** d'une introduction 3D : la structure Next.js, la police
hébergée localement, la palette de couleurs et les métadonnées.
**La scène 3D n'est pas encore intégrée** : la page affiche pour l'instant un
simple texte de vérification de la police.

> [!NOTE]
> Le code de la scène 3D (modèle de l'ordinateur, ouverture du capot, mouvement de
> caméra) se trouve sur la branche `landing-page-header`, qui est la branche
> affichée par défaut du dépôt. Cette branche `main` ne sert que de socle propre.

**Auteur :** Rafaël HOCQUEL
**Version :** 0.2 - socle

## Ce que fera l'introduction (une fois la scène intégrée)

| Étape | Ce qui se passera |
|-------|-------------------|
| 1 | La scène s'ouvre sur un ordinateur portable |
| 2 | Son capot se lève, l'écran s'allume |
| 3 | La caméra avance vers l'écran |
| 4 | L'écran passe au premier plan et le site apparaît, à sa taille normale |
| 5 | Le visiteur se retrouve simplement sur le site, avec sa navigation habituelle |

L'introduction ne se jouera qu'une fois, et restera facultative : un lien direct
vers le site doit toujours être possible, pour les visiteurs pressés comme pour
les moteurs de recherche.

## Comment l'utiliser

| Ce que vous voulez changer | Où |
|---------------------------|-----|
| **Votre site** | Pas encore de dossier dédié : ses fichiers seront servis tels quels une fois la scène intégrée |
| Le titre et la description | `app/layout.tsx` |
| Les couleurs | `app/globals.css`, où la palette est définie en variables |
| La police | `app/fonts`, en la déposant dans le dépôt plutôt qu'en la demandant à un service externe |
| Le logo et la signature | `public/logos` et `public/signatures`, qui contiennent ici des exemples à remplacer |

## Où en est le projet

| Étape | État |
|-------|------|
| Socle Next.js, TypeScript et Tailwind | Fait |
| Police Source Serif 4 hébergée localement | Fait |
| Palette de couleurs en variables | Fait |
| Titre et description du site | Fait |
| Modèle 3D de l'ordinateur et ouverture du capot | À faire |
| Mouvement de caméra et transition vers le site déposé | À faire |
| Version allégée pour les téléphones | À faire |

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
```
