# Projet-IAM-SSO-SIEM
Mise en place d'une infrastructure IAM / SSO avec Keycloak et l'AD, intégration de Grafana et Nextcloud au SSO et attaque MITM sur le trafic LDAP en clair. Puis hardening LDAPS et supervision via l'installation d'un SIEM Wazuh.

Je me forme sur la gestion des identités et des accès (IAM) en construisant une infrastructure complète. L'idée est de comprendre les risques et opportunités de l'implémentation d'un IAM en lab, comprendre ses vulnérabilités et comment sécuriser cet environnement. Suite logique du projet : construction, attaque, durcissement et surveillance.

Ce que j'ai mis en place :
* SSO centralisé via Keycloak fédéré sur un AD Windows Server
* Intégration sur Grafana et Nextcloud avec une gestion des droits basés sur les utilisateurs de l'AD
* Démonstration d'une attaque MITM (Man In The Middle) sur le trafic LDAP en clair pour interception des credentials et énumération complète de l'AD
* Hardening de l'infrastructure via passage en LDAPS pour chiffrer les échanges et rendre l'interception inutile
* Supervision des événements via l'implémentation d'un SIEM Wazuh en configurant des règles de détection personnalisées à l'environnement critique

Stack technique :
* Keycloak
* AD
* Wazuh
* Docker
* Grafana
* Nextcloud
* Kali
* Wireshark
* tcpdump
* ldapsearch

Rapport complet : Le rapport détaillé est disponible dans ce repo, il vise à documenter l'architecture, les problèmes rencontrés, les commandes utilisées ainsi que l'analyse de l'attaque
