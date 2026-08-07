# C2R PulseDeck

## Presentation

C2R PulseDeck est presente ici avec son concept, ses fonctions, ses choix de conception et ses informations d'utilisation.

## Demarrage rapide

### Pre-requis

- Git installe localement.

### Installer et lancer

```powershell
git clone https://github.com/RYJITS/pulsedeck.git
cd pulsedeck
```

## Installation locale

Le depot actuel contient la specification du projet. Cloner le depot, entrer dans le dossier puis ouvrir `projet_c2r_pulsedeck.md`. Aucune installation de dependances n'est necessaire tant que le MVP React n'a pas ete implemente.

### Pre-requis
- Verifier les pre-requis propres au projet dans le README.

### Commandes
```powershell
git clone https://github.com/RYJITS/pulsedeck.git
cd pulsedeck
```

## Lancement

Aucune commande de lancement n'est fournie dans les fichiers publies.

## Utilisation

Dans l'etat actuel, utiliser le depot pour lire et affiner le cahier des charges, definir le perimetre du MVP et suivre les prochaines etapes. Une fois le MVP developpe, le parcours prevu sera: saisir une idee, generer la fiche, la corriger, puis l'exporter en Markdown.

## Concept

Cahier des charges d'une application locale qui doit transformer des idees brutes en fiches projet structurees et exportables en Markdown.

Preparer un MVP capable de clarifier une idee, produire une fiche reutilisable et faciliter sa publication dans un portfolio.

Public vise: Createurs, designers, developpeurs et utilisateurs d'IA qui veulent structurer rapidement leurs idees de projet.


## Fonctionnement de l'application

Le MVP prevu devra proposer une saisie d'idee, transformer cette saisie en blocs structures, conserver les projets dans un fichier JSON local et exporter une fiche Markdown. Les fonctions de tableau de bord, de detection des fiches incompletes et d'assistance IA sont decrites comme des etapes a developper; elles ne sont pas encore implementees dans ce dossier.

## Fonctions de l'application

- Prevoir une saisie rapide d'idee avec titre, categorie, priorite et statut.
- Prevoir la transformation d'une idee en fiche projet structuree.
- Prevoir l'export des fiches au format Markdown.
- Prevoir un stockage local JSON et des statuts de progression.
- Prevoir une description courte et un prompt de vignette pour chaque projet.
- Prevoir un tableau de bord simple pour retrouver les projets et leurs informations manquantes.

## Actualisations et evolution

- Cahier des charges du MVP documente dans projet_c2r_pulsedeck.md
- Depot GitHub public initialise le 7 aout 2026

## Comment le projet a ete reflechi et construit

Le brief propose une application React et TypeScript construite avec Vite et Tailwind CSS, sans backend ni cloud pour le MVP. Les ecrans envisages sont la capture d'idee, la fiche generee et un tableau de bord. La priorite est de valider un parcours simple avant d'ajouter des automatisations ou des effets visuels avances.

### Outils, IA et moteurs utilises

- Markdown pour le cahier des charges
- Git pour versionner la specification
- React, TypeScript, Vite et Tailwind CSS proposes pour le futur MVP
- JSON local propose pour les donnees
- MVP local sans backend
- Separation entre saisie, fiche et tableau de bord
- Export Markdown
- Stockage local JSON
- Fonctions avancees repoussees apres validation du MVP

### Options techniques detectees

- Options techniques a documenter.

### Stack et dependances principales

- Dossier projet
- MVP local sans backend
- Separation entre saisie, fiche et tableau de bord
- Export Markdown
- Stockage local JSON
- Fonctions avancees repoussees apres validation du MVP

### Scripts disponibles

- Aucun script detecte.

### Dependances applicatives

- Aucune dependance applicative detectee.

### Dependances de developpement

- Aucune dependance de developpement detectee.

## Automatisations et comportements internes

- Automatisations a documenter.

## Captures d'ecran

Aucune capture publique n'est disponible pour ce projet.

## Variables d'environnement

Aucune variable d'environnement n'est requise d'apres les fichiers publies.

## Securite

Ne jamais publier `.env`, tokens, sessions, logs sensibles, cles privees ou donnees personnelles.
