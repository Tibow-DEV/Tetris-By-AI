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

🔌 Technologies recommandées

✅ Python (serveur + client)

✅ WebSockets avec FastAPI ou Flask-SocketIO

✅ Pygame pour l'affichage


🏗 Architecture du projet

Serveur (server.py)

Gère la connexion des joueurs

Synchronise les états du jeu (position des pièces, score, etc.)

Envoie les actions de chaque joueur à l’autre

Client (client.py)

Envoie les actions du joueur au serveur

Reçoit les mises à jour de l’état du jeu

Affiche le jeu avec Pygame

🔄 Déroulement du jeu

Les joueurs se connectent au serveur

Chaque joueur joue sur son propre écran

Lorsqu'un joueur supprime des lignes, l’autre reçoit un handicap (lignes supplémentaires)

Le jeu continue jusqu'à ce qu’un joueur perde

💡 On commence par quoi ? Initialiser le serveur ou créer un client test ? 😊

