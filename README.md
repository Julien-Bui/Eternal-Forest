# Eternal Forest — Projet C# (EPITA 1ère Année)

> **Projet académique réalisé en 1ère année à l'EPITA.**  
> Ce dépôt GitHub a pour vocation principale de **présenter le code source et l'architecture C#** dans le cadre d'un portfolio de développeur.

---

## Présentation du Projet

**Eternal Forest** est un jeu de survie et d'exploration 2D développé sous le moteur **Godot 4 (.NET 8 / C#)**.

Ce projet étudiant avait pour objectif de concevoir un jeu vidéo complet de A à Z en équipe, intégrant la génération procédurale, la gestion d'entités, un système d'inventaire, des mécaniques de combat, de la sauvegarde et du multijoueur.

> _Note : Ce dépôt est volontairement allégé (assets graphiques et binaires ignorés) afin de mettre en avant la structure, la logique métier et la propreté du code C#._

---

## Stack Technique

- **Langage :** C# (.NET 8)
- **Moteur :** Godot Engine 4 (Mono / C#)
- **IDE supportés :** JetBrains Rider, Visual Studio, VS Code

---

## Architecture & Organisation du Code

L'architecture logicielle s'articule autour de modules C# modulaires :

```text
Eternal-Forest/
├── Game/                  # Gestionnaire global du cycle de vie du jeu (GameManager)
├── Player/                # Déplacement, contrôleur joueur et suivi de caméra (CameraFollow)
├── Mobs/                  # Comportements des ennemis et logique d'IA (Orc, etc.)
├── Map/                   # Génération de carte et de terrain (map_gen, floor_gen, multi)
├── Inven/                 # Système d'inventaire, objets et barre de raccourcis (Hotbar)
├── Health/                # Gestion des points de vie et feedback visuel
├── Saves/                 # Persistance des données et sauvegarde automatique
├── UI/                    # Menus principaux, sélection solo et lobbies multijoueur
└── scenes/                # Boucles de jeu (GameSolo, GameMultiplayer, GameSaveData)
```

---
