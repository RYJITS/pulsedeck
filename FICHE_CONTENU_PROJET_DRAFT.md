# Brouillon contenu fiche - C2R PulseDeck

## Resume
Cahier des charges d'une application locale qui doit transformer des idees brutes en fiches projet structurees et exportables en Markdown.

## A quoi sert le projet
Preparer un MVP capable de clarifier une idee, produire une fiche reutilisable et faciliter sa publication dans un portfolio.

## Fonctionnement
Le MVP prevu devra proposer une saisie d'idee, transformer cette saisie en blocs structures, conserver les projets dans un fichier JSON local et exporter une fiche Markdown. Les fonctions de tableau de bord, de detection des fiches incompletes et d'assistance IA sont decrites comme des etapes a developper; elles ne sont pas encore implementees dans ce dossier.

## Construction
Le brief propose une application React et TypeScript construite avec Vite et Tailwind CSS, sans backend ni cloud pour le MVP. Les ecrans envisages sont la capture d'idee, la fiche generee et un tableau de bord. La priorite est de valider un parcours simple avant d'ajouter des automatisations ou des effets visuels avances.

## Installation
Le depot actuel contient la specification du projet. Cloner le depot, entrer dans le dossier puis ouvrir `projet_c2r_pulsedeck.md`. Aucune installation de dependances n'est necessaire tant que le MVP React n'a pas ete implemente.

## Utilisation
Dans l'etat actuel, utiliser le depot pour lire et affiner le cahier des charges, definir le perimetre du MVP et suivre les prochaines etapes. Une fois le MVP developpe, le parcours prevu sera: saisir une idee, generer la fiche, la corriger, puis l'exporter en Markdown.

## Fonctions
- Prevoir une saisie rapide d'idee avec titre, categorie, priorite et statut.
- Prevoir la transformation d'une idee en fiche projet structuree.
- Prevoir l'export des fiches au format Markdown.
- Prevoir un stockage local JSON et des statuts de progression.
- Prevoir une description courte et un prompt de vignette pour chaque projet.
- Prevoir un tableau de bord simple pour retrouver les projets et leurs informations manquantes.
