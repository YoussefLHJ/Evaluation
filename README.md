## Tables Overview

### 1. Categories

Stores product categories.

| id | code | libelle  |
|----|------|----------|
| 1  | HW   | Hardware |

---

### 2. Produits (Products)

Stores product information with category references.

| id | reference | prix | categorie_id |
|----|-----------|------|--------------|
| 1  | ES12      | 120  | 1            |
| 2  | ZR85      | 100  | 1            |
| 3  | EE85      | 200  | 1            |

---

### 3. Lignes_commande (Order Lines)

Stores order line items with product references.

| id | quantite | commande_id | produit_id |
|----|----------|-------------|------------|
| 1  | 7        | 1           | 1          |
| 2  | 14       | 1           | 2          |
| 3  | 5        | 1           | 3          |

---

### 4. Employes (Employees)

Stores employee information.

| id | email         | fonction | nom  | prenom | telephone  |
|----|---------------|----------|------|--------|------------|
| 1  | test@test.com | test     | test | test   | 0600000000 |

---

### 5. Projets (Projects)

Stores project information with project manager references.

| id | nom     | dateDebut  | chef_id |
|----|---------|------------|---------|
| 1  | projet1 | 2013-01-14 | 1       |

---

### 6. Taches (Tasks)

Stores project tasks with planned dates and pricing.

| id | nom           | dateDebutPlanifie | dateFinPlanifiee | prix | projet_id |
|----|---------------|-------------------|------------------|------|-----------|
| 1  | Analyse       | 2013-02-05        | 2013-02-28       | 1500 | 1         |
| 2  | Conception    | 2013-03-01        | 2013-03-30       | 2000 | 1         |
| 3  | Developpement | 2013-04-01        | 2013-05-05       | 5000 | 1         |

---

### 7. Femmes (Women)

Stores information about women.

| id | naissance  | adresse | nom    | prenom |
|----|------------|---------|--------|--------|
| 1  | 1970-01-01 | Adr 1   | SALIMA | RAMI   |
| 2  | 1972-02-02 | Adr 2   | AMAL   | ALI    |
| 3  | 1975-03-03 | Adr 3   | WAFA   | ALAOUI |
| 4  | 1971-04-04 | Adr 4   | KARIMA | ALAMI  |

---

### 8. Hommes (Men)

Stores information about men.

| id | naissance  | adresse | nom  | prenom |
|----|------------|---------|------|--------|
| 1  | 1965-01-01 | Adr A   | SAFI | SAID   |

---

### 9. Mariages (Marriages)

Stores marriage records between men and women.

| id | dateDebut  | dateFin    | nbrEnfants | femme_id | homme_id |
|----|------------|------------|------------|----------|----------|
| 1  | 1990-09-03 | NULL       | 4          | 1        | 1        |
| 2  | 1995-09-03 | NULL       | 2          | 2        | 1        |
| 3  | 2000-11-04 | NULL       | 3          | 3        | 1        |
| 4  | 1989-09-03 | 1990-09-03 | 0          | 4        | 1        |
