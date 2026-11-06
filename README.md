# SAS Final Project

A final exam project for YouCode School, Campus Nador 2026.

This project is a command-line student management system built in JavaScript. It allows a training manager or admin to manage learners, record their daily results, track progress, and sort/filter the student list using a simple interactive console menu.

## Project Overview

The application is designed to help manage the progress of students in a coding bootcamp. It provides a lightweight dashboard to:

- view overall student progress
- add new learners
- inspect a learner by ID
- record or update daily exercise results
- search learners by name
- filter learners by level
- sort learners by progression or alphabetically

## Features

- Dashboard summary of student performance
- Display all learners in a clean console table
- Add a new student with personal information
- Consult a student by ID
- Record daily progress and completed exercises
- Search students by name
- Filter learners by level
- Sort by progression descending
- Sort alphabetically
- Exit menu when finished

## Tech Stack

- JavaScript
- Node.js
- ES Modules
- prompt-sync

## Project Structure

```text
SAS-FINAL/
├── main.js
├── data.js
├── package.json
├── package-lock.json
├── services/
│   ├── afficherTableauDeBord.js
│   ├── afficherApprenant.js
│   ├── afficherApprenants.js
│   ├── ajouterApprenant.js
│   ├── calculerProgression.js
│   ├── enregistrerResultat.js
│   ├── filtrerParNiveau.js
│   └── rechercherApprenant.js
├── utilities/
│   ├── prompt.js
│   ├── FindByID.js
│   ├── FindByName.js
│   ├── SortAlphabete.js
│   ├── SortByProgression.js
│   ├── isUserExists.js
│   ├── normaliserNom.js
│   └── validerResultat.js
└── README.md
```

## Main Menu

When you run the app, the console displays a menu like this:

```text
SAS PROGRESS CONSOLE
1. Afficher le tableau de bord
2. Afficher la liste des apprenants
3. Ajouter un apprenant
4. Consulter un apprenant par identifiant
5. Ajouter ou modifier le résultat d'une journée
6. Rechercher un apprenant par nom
7. Filtrer les apprenants par niveau
8. Trier les apprenants par progression décroissante
9. Trier les apprenants par ordre alphabétique
0. exit
```

## Getting Started

### Prerequisites

- Node.js installed on your machine
- npm installed

### Installation

```bash
git clone https://github.com/zakariabensaid-360/SAS-FINAL.git
cd SAS-FINAL
npm install
```

### Run the project

```bash
node main.js
```

## Example of Use

After launching the app, you can:

1. Display the dashboard
2. Add a student to the list
3. Enter daily results for a learner
4. Search by name or filter by level
5. Sort learners by performance or alphabetically

## Data Model

Each student contains:

- id
- nomComplet
- ville
- resultats

Each result includes:

- jour
- exercicesTermines
- totalExercices
- challengeTermine

## Academic Context

This project was developed as part of the final exam for the YouCode School program at the Nador campus in 2026. It reflects the practical application of JavaScript fundamentals, logic building, data manipulation, modular programming, and user interaction via the console.

## Author

Developed by Zakaria Bensaid

## License

ISC

## Future Improvements

Possible upgrades for the project include:

- migrating to TypeScript
- integrating a real database (MySQL/PostgreSQL)
- creating a web interface with React or Next.js
- adding authentication and role-based access
- building a backend API with Express
- storing data permanently instead of in a local JavaScript array

---

Made with passion for the YouCode final project.
