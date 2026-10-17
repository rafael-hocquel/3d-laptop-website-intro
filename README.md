# Intro Web 3D — Ouverture d'un ordinateur portable

Une animation d'introduction en 3D pour un site web : la scène démarre sur un ordinateur portable fermé, l'écran s'ouvre et s'allume, puis la caméra plonge dedans pour laisser place au vrai site en plein écran.

L'idée est de garder l'animation légère et non bloquante : elle ne se joue qu'une seule fois, et on peut toujours la passer ou accéder au site par un lien direct (pratique pour les utilisateurs pressés comme pour le SEO).

> [!NOTE]
> Vous êtes sur la branche `landing-page-header` (branche par défaut), suite au changement d'objectif de ce projet, le code lié à l'animation se trouve sur cette branche, en attendant une migration

## Déroulement de la séquence

1. Apparition de l'ordinateur portable fermé.
2. Ouverture du capot et allumage de l'écran.
3. Travelling de la caméra vers l'écran.
4. Transition plein écran vers le site final, qui prend le relais avec sa navigation classique.

## Personnalisation

Le projet est pensé comme une brique réutilisable. Voici où modifier les éléments principaux :

| Élément | Emplacement | Détails |
| :--- | :--- | :--- |
| **Métadonnées** | `app/layout.tsx` | Titre de la page et description SEO |
| **Couleurs** | `app/globals.css` | Palette définie via des variables CSS |
| **Typographie** | `app/fonts/` | Police hébergée en local (*Source Serif 4* par défaut, sans appel externe) |
| **Assets** | `public/logos/`, `public/signatures/` | Fichiers d'exemple à remplacer par les vôtres |
| **Site cible** | *À venir* | Le dossier dédié au site final sera branché une fois la transition caméra terminée |

## Avancement

- [x] Socle technique (Next.js 16, React 19, TypeScript, Tailwind CSS 4)
- [x] Configuration des variables CSS et hébergement local de la police
- [x] Intégration du modèle 3D et animation d'ouverture du capot
- [ ] Travelling caméra et transition fluide vers le DOM du site
- [ ] Fallback / version allégée pour mobile

## Lancer le projet en local

```bash
git clone https://github.com/rafael-hocquel/3d-laptop-website-intro.git
cd 3d-laptop-website-intro
npm install
npm run dev
