
# data-structures-and-algorithms

## Table des matières
- [Description](#description)
- [Objectif pédagogique](#objectif-pédagogique)
- [Structure du dépôt](#structure-du-dépôt)
- [Problèmes résolus](#problèmes-résolus)
- [Patterns appris](#patterns-appris)
- [Technos utilisées](#technos-utilisées)
- [Notes personnelles](#notes-personnelles)

---

## Description

Ce dépôt contient mon parcours d'apprentissage en algorithmes et structures de données.

L'idée n'est pas seulement de stocker des solutions à des exercices (style LeetCode), mais surtout de documenter :
- les **patterns d'algorithmes** réutilisables (Prefix Sum, HashMap Lookup, Two Pointers, etc.),
- les **structures de données** clés (Array, Set, Map, etc.),
- mon **raisonnement** pour chaque problème.

Le but est de construire un "playbook" réutilisable qui permet de reconnaître un pattern déjà vu et l'appliquer.

---

## Objectif pédagogique

1. Devenir à l'aise avec les tableaux, les boucles, les sommes préfixes, les hashmaps, etc.
2. Comprendre la complexité (temps / espace) de mes solutions.
3. Relier chaque problème à un pattern connu.
4. Préparer progressivement les entretiens techniques (DSA = Data Structures & Algorithms).

---

## Structure du dépôt

```text
data-structures-and-algorithms/
├─ README.md
├─ patterns/
│   ├─ prefix_sum.md                 ← Somme préfixe / running sum / différence gauche-droite
│   ├─ two_pointers.md               ← (à venir)
│   ├─ hash_map_lookup.md            ← (à venir)
│   ├─ hash_set_duplicate_check.md   ← (à venir)
│   ├─ one_pass_min_tracking.md      ← (à venir)
│   └─ 2d_traversal_and_max.md       ← Parcours matrice + max global
├─ data_structures/
│   ├─ array.md                      ← notes sur les tableaux
│   ├─ set.md                        ← notes sur Set / détection de doublons
│   └─ map_hashmap.md                ← notes sur Map / clé → valeur
└─ solutions/
    ├─ running_sum/
    │   ├─ problem.md
    │   └─ solution.js
    ├─ pivot_index/
    │   ├─ problem.md
    │   └─ solution.js
    ├─ richest_customer_wealth/
    │   ├─ problem.md
    │   └─ solution.js
    ├─ contains_duplicate/
    │   ├─ problem.md                ← (à venir)
    │   └─ solution.js               ← (à venir)
    ├─ two_sum/
    │   ├─ problem.md                ← (à venir)
    │   └─ solution.js               ← (à venir)
    └─ best_time_to_buy_and_sell_stock/
        ├─ problem.md                ← (à venir)
        └─ solution.js               ← (à venir)
````

* `patterns/`
  Carnet de patterns : chaque fichier explique une technique d'algo, quand l'utiliser, la complexité typique, et donne une forme générique.

* `data_structures/`
  Notes sur les structures de données que j'utilise (array, set, map, etc.).
  But : comprendre ce qu'elles font et pourquoi elles sont utiles en algorithmique.

* `solutions/`
  Un dossier par problème.
  Chaque problème contient :

  * `problem.md` : résumé du challenge, pattern utilisé, complexité, ce que j'ai appris.
  * `solution.js` : mon code en JavaScript.

---

## Problèmes résolus

| Problème                        | Pattern principal                  | Langage    | Statut      | Dossier                                      |
| ------------------------------- | ---------------------------------- | ---------- | ----------- | -------------------------------------------- |
| Running Sum of 1D Array         | Prefix Sum / Running Prefix Sum    | JavaScript | ✅ Fini      | `solutions/running_sum/`                     |
| Pivot Index                     | Prefix Sum (left sum vs right sum) | JavaScript | ✅ Fini      | `solutions/pivot_index/`                     |
| Richest Customer Wealth         | 2D Traversal + Max Tracking        | JavaScript | ✅ Fini      | `solutions/richest_customer_wealth/`         |
| Contains Duplicate              | Hash Set Duplicate Check           | JavaScript | 🔄 En cours | `solutions/contains_duplicate/`              |
| Two Sum                         | Hash Map Complement Lookup         | JavaScript | ⏳ À faire   | `solutions/two_sum/`                         |
| Best Time to Buy and Sell Stock | One-Pass Min Tracking              | JavaScript | ⏳ À faire   | `solutions/best_time_to_buy_and_sell_stock/` |

Objectif : garder ce tableau à jour pour suivre ma progression.

---

## Patterns appris

Ces patterns sont les “recettes mentales” que je veux reconnaître rapidement quand je lis un énoncé.

| Pattern / Nom (EN)                        | Idée générale                                                                                    | Exercices associés                          |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------ | ------------------------------------------- |
| Prefix Sum / Running Prefix Sum           | Accumuler une info au fur et à mesure pour éviter de recalculer à chaque index.                  | Running Sum of 1D Array, Pivot Index        |
| 2D Traversal + Max Tracking               | Parcourir une matrice ligne par ligne, calculer une valeur locale, garder le max global.         | Richest Customer Wealth                     |
| Hash Set Duplicate Check                  | Utiliser un `Set` pour détecter si une valeur est déjà apparue.                                  | Contains Duplicate                          |
| Hash Map Complement Lookup                | Stocker valeur → index et retrouver le complément de la target en O(1).                          | Two Sum                                     |
| One-Pass Min Tracking                     | Garder le minimum vu jusque-là et calculer le meilleur profit en une seule passe.                | Best Time to Buy and Sell Stock             |
| Two Pointers (Slow/Fast / Merge In-Place) | Avancer deux index à des vitesses / positions différentes pour filtrer, compresser ou fusionner. | Move Zeroes, Merge Sorted Array (plus tard) |
| Kadane’s Algorithm (Max Subarray)         | Garder la meilleure somme locale courante et la meilleure somme globale.                         | Maximum Subarray (plus tard)                |

Chaque pattern a (ou aura) son fichier détaillé dans `patterns/`.

---

## Technos utilisées

* **JavaScript**

  * Toutes les solutions sont écrites en JS pour travailler les algos façon LeetCode.
  * Les idées restent valables dans d'autres langages (Java, Python, etc.).

* **Markdown**

  * La réflexion et les explications sont écrites en Markdown (`.md`) pour être lisibles directement sur GitHub.

---

## Notes personnelles

* Le but de ce repo est l'apprentissage progressif, pas “farmer le plus de problèmes possible”.
* Chaque problème doit être relié à un pattern identifiable.
* L'étape importante n'est pas seulement “j'ai réussi”, c'est “je sais pourquoi ça marche et quand réutiliser l'idée”.



