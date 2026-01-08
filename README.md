# Mise en place d’une solution de sécurité des endpoints et de supervision SIEM avec Wazuh dans un environnement AWS

**Étudiante :** Aya OUZARF  
**Encadrant :** Prof. Azeddine KHIAT  
**Année :** 2025/2026
## 📌 Description du projet
Ce projet présente la mise en place d’une solution de supervision de sécurité
basée sur Wazuh, combinant les approches SIEM et EDR, dans un environnement
multi-OS (Linux et Windows), déployé sur AWS Learner Lab.

L’objectif est de superviser des endpoints, détecter des événements de sécurité
et analyser les alertes via une plateforme centralisée.

## 🎯 Objectif

- Déployer Wazuh All-in-One sur une instance Linux
- Superviser des systèmes Linux et Windows
- Détecter des attaques de type bruteforce, élévation de privilèges et
  modifications de fichiers sensibles
- Utiliser Sysmon pour renforcer la surveillance EDR sur Windows
- Centraliser l’analyse des alertes via le dashboard Wazuh
  
## 🏗️ Architecture

- 1 serveur Wazuh (Ubuntu – All-in-One)
- 1 client Linux (agent Wazuh)
- 1 client Windows (agent Wazuh + Sysmon)
- Hébergement sur AWS EC2


## 📂 Contenu du dépôt
- `configs/` : fichiers de configuration et informations système
- `Rapport.pdf` : captures d’écran de la démonstration
- `screenshots/` : captures d’écran de la démonstration
  

## 🧪 Scénarios testés

1. **SSH Bruteforce** (Linux) : Détection de tentatives échouées
2. **Failed RDP Login** (Windows) : Event ID 4625
3. **User Creation** (Windows) : Event ID 4720 + 4732
4. **Sysmon Events** : Process Creation, Network Connection, File Creation
5. **File Integrity Monitoring** : Modifications de fichiers sensibles

## 🔍 Technologies utilisées

- AWS EC2
- Wazuh 4.7
- Ubuntu 22.04 LTS
- Windows Server 2025
- Sysmon
- Security Groups AWS

## 📹 Vidéo de démonstration

[Lien vers la vidéo - À ajouter]

## 📚 Compétences acquises

- Déploiement infrastructure Cloud sécurisée
- Configuration SIEM (Wazuh)
- Mise en œuvre EDR (Sysmon)
- Détection et analyse d'incidents
- Threat Hunting
