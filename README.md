# gitlab-nginx-monitoring

Solution automatisée basée sur Ansible pour déployer une instance GitLab sécurisée avec Nginx en tant que reverse proxy et Let's Encrypt pour le chiffrement HTTPS.

L’infrastructure est orchestrée avec Docker Compose et inclut un pipeline CI/CD permettant de tester, construire et déployer des applications Dockerisées.

Un système de monitoring et d’alerting est intégré avec Prometheus, Grafana et Alertmanager pour assurer la supervision des services.

✅ Technologies utilisées :

GitLab (gestion du code et CI/CD)
Nginx (reverse proxy, HTTPS)
Let's Encrypt (certificats SSL)
Ansible (automatisation du déploiement)
Docker & Docker Compose (orchestration des services)
Prometheus, Grafana & Alertmanager (monitoring et alerting)
🔧 Prérequis :

Serveur Linux avec un nom de domaine
