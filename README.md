# Projet de Jeu 2D avec LibGDX

## Description du Projet

Ce projet est un jeu en 2D développé en utilisant la bibliothèque LibGDX. Le jeu met en scène un personnage principal (un koala) qui explore plusieurs niveaux tout en affrontant des ennemis. Le joueur peut sauter, marcher, courir, attaquer des ennemis, et doit survivre pour atteindre la fin du niveau. Le projet comprend également un système de menus, des écrans de victoire et de défaite, ainsi qu'une interface pour sélectionner le niveau.

## Fonctionnalités Principales

1. **Personnage Jouable** : Le joueur contrôle un personnage (Koala) avec plusieurs états, comme debout, en marche, sautant, et attaquant. Le joueur peut se déplacer à droite, à gauche, sauter, et attaquer les ennemis.
2. **Ennemis** : Des ennemis sont dispersés dans les différents niveaux. Ils ont des points de vie qui peuvent être réduits lorsque le joueur les attaque. Lorsqu'un ennemi perd tous ses points de vie, il disparaît du niveau.
3. **Niveaux Multiples** : Le jeu inclut plusieurs niveaux avec différents obstacles et ennemis. Le joueur peut sélectionner un niveau à partir du menu de sélection des niveaux.
4. **Système de Pause** : Le joueur peut mettre le jeu en pause à tout moment en appuyant sur la touche "ESCAPE" et accéder à un menu pour reprendre ou retourner au menu principal.
5. **Écrans de Victoire et de Défaite** : Si le joueur vainc tous les ennemis ou atteint certains objectifs, un écran "YOU WIN" est affiché. De même, si le joueur perd, un écran "YOU LOSE" apparaît.
6. **Menu des Options** : Une interface de menu des options est disponible avec des commandes pour régler les différents paramètres du jeu.

## Commandes du Jeu

- **Sauter** : Touche `Espace`
- **Frapper/Attaquer** : Touche `E`
- **Se Déplacer à Droite** : Touche `Flèche Droite`
- **Se Déplacer à Gauche** : Touche `Flèche Gauche`
- **Mettre en Pause** : Touche `ESCAPE`

## Installation et Exécution

1. **Prérequis** :
   - Java Development Kit (JDK) version 8 ou ultérieure.
   - LibGDX installé.

2. **Clôner le dépôt** :
   ```sh
   git clone git@github.com:EpitechMscProPromo2027/T-JAV-501-PAR_11.git
   ```

3. **Compilation et Exécution** :
   Utilisez Gradle pour compiler et exécuter le projet :
   ```sh
   ./gradlew desktop:run
   ```

## Structure du Projet

- **BaseLevelScreen.java** : Classe de base pour gérer les niveaux du jeu. Contient la logique du personnage principal et les fonctions de rendu du niveau.
- **Level2Screen.java** : Classe spécifique pour le niveau 2, avec des ennemis uniques et des événements spéciaux.
- **Enemy.java** : Classe qui gère les ennemis dans le jeu, incluant leur position, leurs points de vie, et la logique de réduction des points de vie.
- **WinScreen.java** : Classe pour l'écran de victoire, avec des boutons pour retourner à la sélection des niveaux.
- **LoseScreen.java** : Classe pour l'écran de défaite, qui offre la possibilité de retourner à la sélection des niveaux.
- **GameMenu.java** : Classe qui gère le menu principal, incluant les options de démarrage du jeu et de sortie.
- **OptionsMenu.java** : Classe gérant l'affichage des options et des commandes du jeu.

