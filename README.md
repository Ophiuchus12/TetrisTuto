# TetrisTuto
Python tuto youtube 


pip 
wheel
pygame


1. Creation environnement python : python3 -m venv .

2. Activation environnement : source /home/corentin/Projects/TetrisTuto/bin/activate

3. Pygame installation : pip install pygame==2.6.0







///////////////////////////////////////////////////////////
tile_rect = pygame.Rect(column*self.cells_size + 1, row*self.cells_size + 1, self.cells_size - 1, self.cells_size - 1)

crée un rectangle à l'aide de pygame.Rect, qui définit une surface rectangulaire dans Pygame. Cette ligne utilise quatre arguments pour initialiser le rectangle. 
Voici une explication détaillée des parenthèses et de leurs rôles dans cette instruction.
Structure des arguments

pygame.Rect(x, y, width, height)

    x: La coordonnée horizontale du coin supérieur gauche du rectangle.
    y: La coordonnée verticale du coin supérieur gauche du rectangle.
    width: La largeur du rectangle.
    height: La hauteur du rectangle.

Explication des calculs dans les parenthèses

    column * self.cells_size + 1 :
        column * self.cells_size : Calcule la position horizontale de la colonne dans une grille où chaque cellule a une taille définie par self.cells_size.
        + 1 : Décale légèrement cette position pour éviter un chevauchement direct ou pour créer une bordure visuelle (par exemple, un espace d'un pixel).

    row * self.cells_size + 1 :
        row * self.cells_size : Calcule la position verticale de la ligne dans une grille, avec une logique similaire.
        + 1 : Décale également la position verticale pour un alignement précis ou une bordure.

    self.cells_size - 1 (pour la largeur et la hauteur) :
        self.cells_size : Représente la taille d'une cellule dans la grille.
        - 1 : Réduit légèrement la largeur et la hauteur du rectangle pour éviter qu'il ne touche exactement les bords voisins 
        (utilisé pour espacement visuel ou stylisation).