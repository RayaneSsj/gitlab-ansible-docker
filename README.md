# Déploiement GitLab avec Ansible et Docker
Ce projet automatise le déploiement de GitLab sur une VM via Ansible et Docker.

## Pré-requis
- Ansible
- Docker et Docker Compose
- Une VM avec une IP fixe (exemple : `192.168.45.131`).

## Étapes
1. Clonez ce repository sur votre machine hôte.
2. Vérifiez votre inventaire dans `inventory`.
3. Lancez le playbook avec :
   ```bash
   ansible-playbook -i inventory site.yml --ask-become-pass
