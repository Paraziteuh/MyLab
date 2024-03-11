# MyLab
SOC maison

![Untitled](https://github.com/Paraziteuh/MyLab/assets/123948801/85fd9e66-a577-4a4d-b095-1491d6057f1a)


**1. Wazuh Agent:**

- Installé sur les postes clients (Windows 10 dans ce cas), il surveille l'activité du système et envoie des événements à Wazuh Manager.
- Envoie les événements à Wazuh Manager.

**2. Wazuh Manager:**

- Collecte les événements des agents Wazuh.
- Corrélationne les événements pour identifier les menaces potentielles.
- Déclenche des alertes et envoie des notifications aux outils de réponse aux incidents (TheHive et Shuffle).
- Exécute des actions de réponse aux incidents prédéfinies.

**3. TheHive:**

- Plateforme de gestion des incidents.
- Crée des incidents à partir des alertes de Wazuh.
- Enrichit les incidents avec des informations provenant d'autres sources (OSINT).
- Permet aux analystes SOC de collaborer sur les incidents.

**4. Shuffle:**

- Plateforme de réponse aux incidents.
- Automatisation des tâches de réponse aux incidents.
- Envoie des notifications par email et d'autres canaux.
- Exécute des actions de correction sur les systèmes compromis.

**5. IOCs:**

- Indicateurs de compromission (IOC) stockés dans une base de données.
- Utilisés par Wazuh pour identifier les menaces potentielles.
- Enrichis par TheHive avec des informations supplémentaires.

**6. Routeur:**

- Connecte le réseau local à Internet.
- Permet le passage du trafic réseau entre les différents éléments du schéma.

**7. Email:**

- Utilisé pour envoyer des notifications aux analystes SOC.
- Utilisé par Shuffle pour envoyer des rapports et des alertes.

**8. Réponse à incidents:**

- Désigne les actions prises par les analystes SOC pour répondre aux incidents détectés.
- Les actions peuvent inclure la mise en quarantaine des systèmes infectés, la suppression des logiciels malveillants et la restauration des données compromises.
