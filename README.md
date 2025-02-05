# gitlab-nginx-monitoring

Ce projet est une solution automatisée basée sur Ansible pour déployer une instance GitLab sécurisée, avec Nginx en reverse proxy et Let's Encrypt pour le chiffrement HTTPS. L’infrastructure est orchestrée avec Docker Compose, et un système de monitoring est intégré avec Prometheus, Grafana et Alertmanager.

## 📌 Fonctionnalités principales
* Déploiement automatisé de GitLab via Ansible  
* Sécurisation avec Nginx et Let's Encrypt  
* Monitoring avancé avec Prometheus, Grafana et Alertmanager  
* GitLab Runner installé et configuré pour exécuter les pipelines CI/CD


## ⚡ CI/CD

Les pipelines CI/CD sont gérés directement dans un projet GitLab dédié.
Ce repository n'inclut pas le fichier .gitlab-ci.yml, mais il installe et configure un GitLab Runner pour exécuter les pipelines définis dans le projet.

Pour illustrer cette infrastructure, j’ai utilisé une application Python, dans laquelle j’ai intégré un pipeline définissant les étapes d’intégration, de build et de déploiement.

🔗 Lien vers le repository CI/CD : https://github.com/pierreflw/python-gitlab-ci


## ✅ Technologies utilisées

* GitLab  
* Ansible  
* Docker & Docker Compose  
* Nginx  
* Let's Encrypt  
* Prometheus  
* Grafana  
* Alertmanager  


## 🔧 Prérequis

* Un serveur Linux  
* Un nom de domaine pointant vers le serveur   
* Accès SSH avec un utilisateur sudo   
* Ansible installé  


## 🚀 Installation & Utilisation

### 1️⃣ Cloner le repository

git clone https://github.com/pierreflw/gitlab-nginx-monitoring.git  
cd gitlab-nginx-monitoring

### 2️⃣ Modifier l’inventaire Ansible
L'inventaire est défini dans inventory/hosts.yml. Vous devez l’adapter à votre serveur en modifiant l’hôte et les paramètres Ansible.

### 3️⃣ Lancer le déploiement
Une fois l’inventaire configuré, exécutez :

ansible-playbook -i inventory playbook.yml

### 4️⃣ Accéder à GitLab
Une fois l’installation terminée, rendez-vous sur :
➡️ https://domaine.com (ou IP)
