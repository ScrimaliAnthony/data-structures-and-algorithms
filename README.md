# data-structures-and-algorithms

## Table des matières

* [Description](#description)
* [Objectif pédagogique](#objectif-pédagogique)
* [Structure du dépôt](#structure-du-dépôt)
* [Patterns appris](#patterns-appris)
* [Problèmes résolus](#problèmes-résolus)
* [Technos utilisées](#technos-utilisées)
* [Notes personnelles](#notes-personnelles)

---

## Description

Ce dépôt contient mon parcours d'apprentissage en algorithmes et structures de données.

C'est ici que je compilerai mes solutions à des exercices LeetCode mais surtout, que je documenterai :

* les **patterns d'algorithmes** réutilisables,
* les **structures de données** clés,
* mon **raisonnement** pour chaque problème.

Le but est de construire un "playbook" réutilisable qui permet de reconnaître un pattern déjà vu et l'appliquer.

---

## Objectif pédagogique

1. Découvrir et comprendre les principaux **patterns d'algorithmes** et **structures de données**.
2. Comprendre la **complexité temps / espace** de chaque solution et être capable de l'expliquer clairement.
3. Relier chaque problème à **un pattern identifié**, au lieu de le traiter comme un cas isolé.
4. Avancer vers les **entretiens techniques** (DSA = Data Structures & Algorithms) en construisant une base réutilisable plutôt qu'un tas de solutions jetables.

---

## Structure du dépôt

```text
data-structures-and-algorithms/
├─ README.md
├─ patterns/            ← Patterns d'algorithmes réutilisables
├─ data_structures/     ← Notes sur les structures de données
└─ solutions/           ← Un dossier par problème résolu
```

* `patterns/`
  Carnet de patterns d'algorithmes : idée générale, quand l'utiliser, complexité typique, et exemples de problèmes associés.

* `data_structures/`
  Notes sur les structures de données utilisées dans les solutions : rôle, opérations importantes, coûts en temps / espace mémoire.

* `solutions/`
  Un dossier par problème. Chaque problème contient :

  * `problem.md` : résumé du challenge, pattern utilisé, complexité, ce que j'ai appris.
  * `solution.js` : mon code en JavaScript.

---

## Patterns appris

| Pattern / Nom (EN)                                              | Idée générale                                                                                               | Exercices associés                                                                                           |
| --------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| [Prefix Sum / Running Prefix Sum](patterns/prefix_sum.md)       | Accumuler progressivement une information (par ex. la somme) pour éviter de la recalculer à chaque index.   | [Running Sum of 1D Array](solutions/running_sum/problem.md), [Pivot Index](solutions/pivot_index/problem.md) |
| [2D Traversal + Max Tracking](patterns/2d_traversal_and_max.md) | Parcourir une matrice ligne par ligne, calculer une valeur locale, puis garder la meilleure valeur globale. | [Richest Customer Wealth](solutions/richest_customer_wealth/problem.md)                                      |

---

## Problèmes résolus

| Nom du problème                                                         | Pattern utilisé                                                 | Langage    | Dossier                              |
| ----------------------------------------------------------------------- | --------------------------------------------------------------- | ---------- | ------------------------------------ |
| [Running Sum of 1D Array](solutions/running_sum/problem.md)             | [Prefix Sum / Running Prefix Sum](patterns/prefix_sum.md)       | JavaScript | `solutions/running_sum/`             |
| [Pivot Index](solutions/pivot_index/problem.md)                         | [Prefix Sum / Running Prefix Sum](patterns/prefix_sum.md)       | JavaScript | `solutions/pivot_index/`             |
| [Richest Customer Wealth](solutions/richest_customer_wealth/problem.md) | [2D Traversal + Max Tracking](patterns/2d_traversal_and_max.md) | JavaScript | `solutions/richest_customer_wealth/` |

---

