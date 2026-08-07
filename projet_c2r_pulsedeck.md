# Projet : C2R PulseDeck

## 1. Résumé du projet

**C2R PulseDeck** est une application web locale qui transforme automatiquement des idées, notes, captures d’écran et petits textes en fiches visuelles prêtes à publier sur un site portfolio, une page projet ou un réseau social.

L’objectif est simple : éviter de perdre les bonnes idées, les structurer rapidement, puis générer une fiche claire avec :
- un titre fort ;
- une description compréhensible ;
- les outils utilisés ;
- les étapes du projet ;
- les améliorations possibles ;
- une vignette ou une direction visuelle ;
- une version courte pour publication.

Le projet sert de pont entre le cerveau personnel, Codex, les projets locaux et le site C2R.

---

## 2. Problème à résoudre

Actuellement, les idées arrivent souvent sous forme de notes rapides, captures, prompts, bouts de code ou discussions. Le problème est que beaucoup d’idées restent dispersées et ne deviennent jamais des projets visibles ou exploitables.

Le vrai besoin n’est pas seulement de créer plus de choses, mais de mieux transformer ce qui existe déjà en contenu clair, organisé et publiable.

---

## 3. Objectif principal

Créer une application qui permet de prendre une idée brute et de la convertir en fiche projet propre, prête à être intégrée dans un site comme **Ma Méthode**, un portfolio ou une base de projets personnelle.

---

## 4. Public cible

Le projet est conçu pour :
- les créateurs qui ont beaucoup d’idées mais peu de structure ;
- les designers qui veulent présenter leurs projets rapidement ;
- les développeurs qui veulent documenter leurs applications ;
- les personnes qui utilisent l’IA pour accélérer leur travail ;
- C2R, comme outil interne de clarification et de publication.

---

## 5. Concept général

L’utilisateur ajoute une idée dans l’application sous forme de texte libre.

Exemple :

> J’ai une idée d’application qui analyse mes projets locaux et crée automatiquement des fiches pour mon site.

L’application transforme ensuite cette idée en plusieurs blocs :

1. **Résumé clair**
2. **Objectif**
3. **Fonctionnalités**
4. **Public cible**
5. **Outils utilisés**
6. **Structure technique**
7. **Version courte pour le site**
8. **Prompt image pour la vignette**
9. **Checklist Codex**
10. **Statut du projet**

---

## 6. Fonctionnalités principales

### 6.1 Capture rapide d’idée

L’utilisateur peut saisir une idée brute sans devoir la structurer dès le départ.

Champs possibles :
- titre provisoire ;
- texte libre ;
- catégorie ;
- priorité ;
- statut ;
- lien éventuel ;
- capture ou image éventuelle.

---

### 6.2 Transformation automatique en fiche projet

L’application génère une fiche standardisée avec une structure claire :

```md
# Nom du projet

## Résumé
## Problème
## Solution
## Fonctionnalités
## Outils utilisés
## Étapes de développement
## Améliorations possibles
## Version courte pour le site
```

---

### 6.3 Génération de description pour site web

L’application produit une version courte, lisible et orientée utilisateur.

Important : la description doit expliquer ce que fait le projet, pas seulement ce que fait le code.

Exemple :

> C2R PulseDeck transforme des idées brutes en fiches projet claires et prêtes à publier, afin de mieux valoriser les créations, les prototypes et les outils développés avec l’IA.

---

### 6.4 Génération de prompt pour vignette

Pour chaque projet, l’application propose un prompt d’image adapté au style C2R.

Style recommandé :
- fond sombre ;
- contraste rouge, blanc et noir ;
- objet central minimaliste ;
- rendu premium ;
- ambiance technologique ;
- pas de texte lisible dans l’image.

Exemple de prompt :

> Futuristic minimal dashboard object floating in a deep black environment, premium graphite material, red glowing accents, clean composition, cinematic lighting, C2R design style, no readable text.

---

### 6.5 Export Markdown

Chaque fiche peut être exportée en fichier `.md`.

Nom du fichier recommandé :

```txt
YYYY-MM-DD_nom-du-projet.md
```

Exemple :

```txt
2026-06-28_c2r-pulsedeck.md
```

---

### 6.6 Statut de progression

Chaque projet peut avoir un statut :

- Idée brute
- À clarifier
- En cours
- Prototype
- À tester
- Prêt à publier
- Archivé

---

## 7. Fonctionnalités secondaires

### 7.1 Tableau de bord

Un tableau de bord affiche :
- nombre d’idées brutes ;
- nombre de projets en cours ;
- nombre de projets prêts à publier ;
- nombre de projets archivés ;
- projets sans vignette ;
- projets sans description courte.

---

### 7.2 Détection des projets incomplets

L’application peut signaler les fiches qui n’ont pas encore :
- de résumé clair ;
- de public cible ;
- d’image ;
- d’outils listés ;
- de version courte ;
- de prochaine action.

---

### 7.3 Mode “Codex”

Un bouton génère une checklist directement utilisable par Codex.

Exemple :

```md
## Mission Codex

1. Lire la fiche projet.
2. Vérifier si le dossier du projet existe.
3. Si le dossier n’existe pas, le créer.
4. Générer une structure propre.
5. Créer un README.md.
6. Créer une première maquette fonctionnelle.
7. Préparer une description courte pour le site.
8. Proposer deux idées de vignette.
```

---

## 8. Structure technique proposée

### Frontend

- React
- TypeScript
- Tailwind CSS
- Vite

### Données locales

Au départ, les données peuvent être stockées dans un fichier JSON local.

Exemple :

```json
{
  "projects": [
    {
      "id": "c2r-pulsedeck",
      "title": "C2R PulseDeck",
      "status": "Idée brute",
      "category": "IA / Organisation",
      "createdAt": "2026-06-28"
    }
  ]
}
```

### IA

L’IA peut être utilisée pour :
- reformuler les idées ;
- générer les fiches ;
- créer les descriptions ;
- proposer les prompts d’image ;
- générer les checklists Codex.

---

## 9. Structure de dossiers recommandée

```txt
C2R_PulseDeck/
│
├── README.md
├── package.json
├── index.html
│
├── src/
│   ├── main.tsx
│   ├── App.tsx
│   ├── components/
│   │   ├── IdeaInput.tsx
│   │   ├── ProjectCard.tsx
│   │   ├── ProjectEditor.tsx
│   │   ├── Dashboard.tsx
│   │   └── ExportButton.tsx
│   │
│   ├── data/
│   │   └── projects.json
│   │
│   ├── utils/
│   │   ├── generateMarkdown.ts
│   │   ├── slugify.ts
│   │   └── projectStatus.ts
│   │
│   └── styles/
│       └── globals.css
│
└── exports/
    └── markdown/
```

---

## 10. Design visuel

Le design doit rester simple, sombre et efficace.

### Style

- fond noir ou graphite ;
- cartes semi-transparentes ;
- bordures rouges fines ;
- typographie claire ;
- boutons minimalistes ;
- ambiance tableau de bord premium.

### Palette

```txt
Noir profond : #050505
Graphite : #151515
Rouge C2R : #ff1f1f
Blanc : #ffffff
Gris texte : #b8b8b8
```

---

## 11. Écrans principaux

### Écran 1 — Capture d’idée

Objectif : écrire rapidement une idée sans friction.

Éléments :
- champ texte libre ;
- bouton “Transformer en fiche” ;
- choix de catégorie ;
- choix de priorité.

---

### Écran 2 — Fiche générée

Objectif : vérifier et modifier la fiche.

Éléments :
- résumé ;
- problème ;
- solution ;
- fonctionnalités ;
- outils ;
- prochaine action ;
- bouton export Markdown.

---

### Écran 3 — Tableau de bord

Objectif : visualiser l’état des projets.

Éléments :
- cartes de statistiques ;
- liste des projets ;
- filtres par statut ;
- filtres par catégorie ;
- indicateur projets incomplets.

---

## 12. Première version MVP

La première version doit rester simple.

### À faire dans le MVP

- Créer l’interface de saisie d’idée.
- Créer une carte projet.
- Générer une fiche Markdown.
- Exporter la fiche en `.md`.
- Stocker les projets dans un JSON local.
- Ajouter les statuts de progression.
- Ajouter un bouton “copier la fiche”.

### À ne pas faire tout de suite

- Authentification utilisateur.
- Base de données complexe.
- Système cloud.
- Paiement.
- Multi-utilisateur.
- Animations WebGL lourdes.

---

## 13. Améliorations futures

- Connexion au dossier local `D:\00_Cerveau_IA\Projet`.
- Analyse automatique des dossiers existants.
- Création automatique de fiches projet manquantes.
- Génération de vignettes.
- Détection des projets abandonnés.
- Archivage des projets inutilisés.
- Synchronisation avec le site Ma Méthode.
- Mode “audit projet”.
- Mode “préparation publication”.
- Mode “planning d’amélioration”.

---

## 14. Risques et limites

### Risque 1 — Projet trop large

Si le projet essaie de tout faire dès le départ, il risque de devenir lourd et jamais terminé.

**Solution :** commencer uniquement avec la capture d’idée et l’export Markdown.

### Risque 2 — Trop d’automatisation

Tout automatiser peut produire des fiches génériques.

**Solution :** garder une étape de validation humaine.

### Risque 3 — Design trop complexe

Un design trop ambitieux peut ralentir le développement.

**Solution :** créer d’abord une interface simple et propre, puis ajouter les effets visuels ensuite.

---

## 15. Critères de réussite

Le projet est réussi si :

- une idée brute peut devenir une fiche claire en moins de 2 minutes ;
- chaque fiche peut être exportée en Markdown ;
- les projets sont faciles à retrouver ;
- les descriptions sont compréhensibles par quelqu’un qui ne connaît pas le code ;
- l’outil donne envie de documenter les projets au lieu de repousser cette tâche.

---

## 16. Pitch court

**C2R PulseDeck** est un outil local qui transforme les idées brutes en fiches projet claires, structurées et prêtes à publier. Il aide à organiser les créations, documenter les prototypes et préparer rapidement du contenu propre pour un site ou un portfolio.

---

## 17. Instruction courte pour Codex

Créer une application React + TypeScript appelée **C2R PulseDeck**.

Objectif : permettre à l’utilisateur de saisir une idée brute, de la transformer en fiche projet structurée, puis de l’exporter en Markdown.

Contraintes :
- interface sombre style C2R ;
- stockage local en JSON ;
- export `.md` ;
- structure simple ;
- code propre ;
- pas de backend au MVP ;
- pas de cloud ;
- pas d’API payante obligatoire.

Priorité :
1. Interface de saisie.
2. Génération de fiche.
3. Carte projet.
4. Export Markdown.
5. Tableau de bord simple.
