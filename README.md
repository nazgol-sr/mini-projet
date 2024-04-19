# Mini projet LIFAMI

## The Particle Panic


## Sarbakhshian Nazgol P2306823


## L'objectif
L'objectif de _**The Particle Panic**_ est de proposer une expérience ludique dans laquelle le joueur contrôle un objet représenté par une forme géométrique pour éviter les obstacles et entrer en collision avec l'objet au sommet pour marquer des points.

Voici les principales caractéristiques:

* **Contrôle des objets:**
     - Le joueur choisit la forme de l'objet (circulaire, carré ou triangulaire) ainsi que la couleur de l'objet (rouge, bleu ou vert) et peut le contrôler à l'aide des touches directionnelles gauche et droite du clavier. La touche "haut" permet de sauter.
     - Un deuxième objet se déplace automatiquement de gauche à droite de l'écran.

* **Évitez les obstacles:**
     - Les obstacles sont représentés par des trous dispersés sur l'écran.
     - le joueur peut choisir le niveau de difficulté du jeu, qui est directement lié au nombre de trous/obstacles.
     - Le joueur doit manœuvrer le premier objet pour éviter de tomber dans les trous et il doit entrer en collision avec le deuxième objet.

* **Marquer des points:**
     - Chaque fois que le joueur parvient à éviter un trou et à entrer en collision avec l'objet situé au sommet, il marque des points.
     - En revanche, si le joueur entre en collision avec un trou, il perd des points.

* **Terminez le jeu:**
     - Le jeu se termine lorsque le temps imparti est écoulé.
     - A la fin de la partie, le score du joueur est affiché et il est déclaré gagnant s'il a réussi à marquer des points ou perdant s'il n'a pas réussi à marquer de points ou si son score est négatif.
     
## Explication de code
* **Les bibliothèques utilisées dans le code:**
     - _iostream_ : Entrées/sorties standard en C++.
     - _ctime_ : Gestion du temps en C++.
     - _cmath_ : Fonctions mathématiques en C++.
     - _Grapic.h_ : Bibliothèque graphique pour la création d'interfaces graphiques en C++.
* **Initialisation des structures et constantes:**
  - Le code commence par définir des structures (Vec, Hole, Color, Shape) pour représenter des vecteurs, des trous, des couleurs et des formes, ainsi que des constantes pour définir les dimensions de la fenêtre, le pas de temps, le facteur de ralentissement, la gravité et la limite de temps.
* **Fonctions utilitaires:**
  - Le code définit plusieurs fonctions utilitaires pour créer des vecteurs (makeVec), effectuer des opérations sur les vecteurs (operator+, operator-, operator*), générer des nombres aléatoires (frand) et initialiser les formes et les trous (initShape, initShape2, initHoles).
* **Fonctions de dessin et de mise à jour:**
  - Le code contient des fonctions pour dessiner les formes (drawShape, drawShape2) et mettre à jour leur état physique (updateShape, addForce, updateWithKeys). Ces fonctions utilisent les bibliothèques graphiques pour dessiner des formes et gérer les interactions avec l'utilisateur.
* **Gestion des entrées utilisateur:**
   - Le code demande à l'utilisateur de choisir la couleur et la forme de la première particule, ainsi que le niveau de difficulté du jeu.
* **Boucle principale du jeu:**
  - Le code exécute une boucle principale où il met à jour et dessine les formes, gère les entrées de l'utilisateur, détecte les collisions entre les formes et les trous, et affiche le score et le résultat du jeu à la fin du temps imparti.

## Parcours
### Première semaine
Pendant la première semaine, j'ai écrit les fonctions pour dessiner les cercles et les faire bouger. La première était la cible en haut de la page, qui se déplaçait horizontalement, et la seconde était celle que le joueur pouvait contrôler avec la position de la souris. Le joueur peut également utiliser la touche haut du clavier pour entrer en collision avec la cible en haut de la page. Le plus difficile pour moi était que je n'arrivais pas à faire rebondir la particule, et elle montait très vite, donc j'ai dû modifier la vitesse.

### Deuxième semaine
Au cours de la deuxième semaine, j'ai réussi à appliquer la gravité à la particule et à la faire rebondir. J'ai également ajouté une option permettant au joueur de choisir la couleur de la particule. Je voulais également laisser le joueur choisir la forme de la particule, ce que j'ai fait la troisième semaine.

### Troisième semaine
Au cours de la troisième semaine, j'ai réussi à dessiner différentes formes (cercle, rectangle et triangle) et j'ai demandé au joueur de choisir entre eux. J'ai également ajouté des trous (obstacles) cette semaine et j'ai laissé le joueur choisir le niveau de difficulté du jeu (facile, moyen et difficile) qui indiquait le nombre d'obstacles. Vers la fin, j'ai changé toute la structure de mon code, car il était difficile pour C5 de l'exécuter sans aucun bug et mon code était trop long. Au lieu d'écrire chaque fonction pour chaque forme, j'ai écrit une structure de forme qui contenait toutes les formes (presque comme une structure mondiale).

## Resources
  - [Une vidéo YouTube](https://www.youtube.com/watch?v=AWDYJma5bmE) Cette vidéo utilisait SFML qui n'était pas utile pour moi mais cela m'a inspiré pour ce jeu et m'a aidé à comprendre quelle était la structure générale du jeu
  - [Le site de Grapic](https://perso.liris.cnrs.fr/alexandre.meyer/grapic/html/)

  - [C++ Documentation](https//en.cppreference.com/w/)
  - Les codes enseignés au cours du LIFAMI au cours du semestre
  - L'un de mes amis en BAC+4 d'informatique
  



