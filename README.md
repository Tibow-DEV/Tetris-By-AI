# Tetris-By-AI
Projet tetris en utilisant exclusivement de l'IA
📄 Cahier des charges – Tetris en Python
Présentation du projet
1.1 Objectifs
Développer un jeu de Tetris en Python, jouable en solo avec une interface simple et fluide. Le projet pourra évoluer pour inclure un mode multijoueur en ligne et un système de scores enregistrés.

1.2 Fonctionnalités principales
✅ Jeu de Tetris classique avec chute des pièces et rotation
✅ Interface graphique avec Pygame
✅ Système de score et niveaux
✅ Gestion des collisions et suppression des lignes
✅ Sauvegarde du score dans un fichier ou base de données
✅ Mode multijoueur en ligne (optionnel, à ajouter plus tard)

Technologies utilisées
Langage : Python 3
Bibliothèque principale : Pygame (affichage et gestion du jeu)
Stockage des scores : SQLite ou fichier JSON
Multijoueur (optionnel) : WebSockets (avec FastAPI ou Flask-SocketIO)
Architecture du code
main.py → Lance le jeu
tetris.py → Gère la logique du jeu (déplacements, rotations, collisions)
ui.py → Affichage graphique avec Pygame
score_manager.py → Enregistre et charge les scores
(optionnel : network.py pour le mode en ligne)
Déroulement du projet
🔹 Étape 1 : Initialisation du projet et affichage du plateau de jeu
🔹 Étape 2 : Implémentation des blocs et des déplacements
🔹 Étape 3 : Gestion des collisions et suppression des lignes
🔹 Étape 4 : Ajout du score et des niveaux
🔹 Étape 5 : Interface utilisateur améliorée (effets, animations)
🔹 Étape 6 (optionnelle) : Mode multijoueur en ligne
