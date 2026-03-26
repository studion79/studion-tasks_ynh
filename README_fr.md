# Task App pour YunoHost

[![Niveau d'intégration](https://apps.yunohost.org/badge/integration/task_app)](https://ci-apps.yunohost.org/ci/apps/task_app/)
[![Installer Task App avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=task_app)

*[Read this readme in english.](./README.md)*

> *Ce package vous permet d'installer Task App rapidement et simplement sur un serveur YunoHost.*
> *Si vous n'avez pas YunoHost, consultez [ce guide](https://yunohost.org/install) pour savoir comment l'installer.*

## Vue d'ensemble

Task App est un outil de gestion de tâches et d'équipes multi-projets. Il permet d'organiser le travail en projets avec des groupes et des tâches, d'assigner des responsables, de suivre l'avancement via les champs statut et priorité, et de collaborer via des commentaires et des notifications. Plusieurs vues sont disponibles : tableur, Kanban, calendrier, Gantt, fiches et échéancier.

**Version incluse :** 0.1.0

## Fonctionnalités

- Espace de travail multi-projets avec gestion des rôles (Admin / Membre)
- Tâches avec champs statut, priorité, responsable, échéance, timeline, budget et notes
- Vues Kanban, calendrier, Gantt, fiches et échéancier
- Sous-tâches, dépendances et tâches récurrentes
- Commentaires avec @mentions et journal d'activité
- Pièces jointes par tâche
- Tableau de bord personnel avec vue transverse des tâches
- Templates de projet et vues sauvegardées
- Palette de commandes (⌘K)

## Configuration

Après l'installation, créez votre premier compte via la page d'inscription (`/register`).

Pour activer les notifications par e-mail, renseignez `RESEND_API_KEY` dans le fichier `.env` de l'application :

```
/var/www/task_app/.env
```

## Documentations et ressources

- YunoHost Store : <https://apps.yunohost.org/app/task_app>
- Signaler un bug : <https://github.com/studion79/studion-tasks_ynh/issues>

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche `testing`](https://github.com/studion79/studion-tasks_ynh/tree/testing).

Pour tester la branche `testing` :

```bash
sudo yunohost app install https://github.com/studion79/studion-tasks_ynh/tree/testing --debug
```

ou

```bash
sudo yunohost app upgrade task_app -u https://github.com/studion79/studion-tasks_ynh/tree/testing --debug
```
