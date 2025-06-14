# DevOps TP Project

## Description
Application Node.js simple pour le TP DevOps :
- Déploiement via Docker
- Pipeline CI/CD avec GitLab CI

## Lancer l'application
```bash
docker build -t devops-tp-app .
docker run -p 3000:3000 devops-tp-app
```

## Pipeline CI/CD
- Build, test, et déploiement automatisés
- Voir `.gitlab-ci.yml`