# Licence

Calcul des moyennes des UE du BUT 1 R&T (R1.07 - Fondamentaux de la programmation).

Le but : à partir des notes des 15 ressources (R101 à R115) et des 6 SAE (SAE11 à SAE16), calculer la moyenne de chaque UE avec ses coefficients.

## Fichiers

### Calcul_UE.ipynb : calcul des moyennes des 3 UE

- **Version 1** : les notes et les coefficients sont demandés au clavier avec `input()`, une boucle `for` par type de matière.
- **Version 2** : les notes et les coefficients sont rangés dans des listes. Une fonction `moyenne()` calcule la moyenne d'une UE.
- **Version 3** : les notes et les coefficients sont rangés dans des dictionnaires (clé = nom de la matière). Une fonction `dico()` crée les dictionnaires.

### Tkinter.ipynb : interface graphique

- Premier programme : une zone de saisie et un bouton qui ajoute 3 au nombre tapé.
- Programme simplifié : une zone de saisie pour chaque matière, un bouton **Valider**, puis affichage des 3 moyennes.
- Programme de la prof : même principe, avec `numpy` pour la moyenne pondérée.

Corrections faites :
- si une case était vide ou si on tapait une virgule (`12,5`), le programme plantait au clic. Maintenant la virgule est acceptée et une case vide affiche « Il manque une note ! » ;
- la fenêtre du programme de la prof était trop haute : SAE15 et SAE16 étaient coupées sur un écran de portable. J'ai réduit l'espace entre les lignes.

### Graphique_UE.ipynb : graphique des moyennes

Les 3 moyennes sont affichées dans un graphique en barres avec `matplotlib` :
- vert : moyenne ≥ 10
- orange : entre 8 et 10
- rouge : moyenne < 8

- **Version 1** : les notes sont dans une liste.
- **Version 2** : on tape les notes dans une fenêtre Tkinter, puis on clique sur **Calculer**.

Fonctions utilisées : `moyenne_ue()`, `code_couleur()`, `afficher_graphique()`, `creer_zones()`.

## Modules utilisés

`tkinter`, `numpy` et `matplotlib`.

## Auteur

Hévy Poulolo - BUT 1 R&T, groupe B
