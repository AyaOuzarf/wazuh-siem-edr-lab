# Atelier Sécurité des Endpoints et Supervision SIEM avec Wazuh

**Étudiante :** Aya OUZARF  
**Encadrant :** Prof. Azeddine KHIAT  
**Année :** 2025/2026

## 🎯 Objectif

Mise en œuvre d'une plateforme SIEM/EDR complète avec Wazuh sur AWS, supervisant des endpoints Linux et Windows.

## 🏗️ Architecture

- **Wazuh Server** (Ubuntu 22.04) : Manager + Indexer + Dashboard
- **Linux Client** (Ubuntu 22.04) : Agent Wazuh
- **Windows Client** (Windows Server 2025) : Agent Wazuh + Sysmon

## 📁 Structure du projet
```
├── configs/               # Fichiers de configuration
│   ├── ossec_linux.conf
│   ├── ossec_manager.conf
│   ├── local_rules.xml
│   └── sysmonconfig.xml (à ajouter)
├── screenshots/           # Captures d'écran
│   ├── architecture/
│   ├── wazuh_dashboard/
│   ├── linux_events/
│   ├── windows_events/
│   └── sysmon_events/
└── README.md
```

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
