# Task App for YunoHost

[![Integration level](https://apps.yunohost.org/badge/integration/task_app)](https://ci-apps.yunohost.org/ci/apps/task_app/)
[![Install Task App with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=task_app)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Task App quickly and simply on a YunoHost server.*
> *If you don't have YunoHost, please consult [the guide](https://yunohost.org/install) to learn how to install it.*

## Overview

Task App is a cross-project task and team management tool. It lets you organise work into projects with groups and tasks, assign owners, track progress via status and priority fields, and collaborate with teammates through comments and notifications. Multiple views are available: spreadsheet, Kanban, calendar, Gantt, cards, and timeline.

**Shipped version:** 0.1.0

## Features

- Multi-project workspace with role-based access (Admin / Member)
- Tasks with status, priority, owner, due date, timeline, budget, and notes fields
- Kanban, calendar, Gantt, cards, and timeline views
- Subtasks, task dependencies, recurring tasks
- Comments with @mentions and activity log
- File attachments per task
- Personal dashboard with cross-project task overview
- Project templates and saved views
- Command palette (⌘K)

## Configuration

After installation, create your first account via the registration page (`/register`).

To enable email notifications, set `RESEND_API_KEY` in the app's `.env` file:

```
/var/www/task_app/.env
```

## Documentation and resources

- YunoHost Store: <https://apps.yunohost.org/app/task_app>
- Report a bug: <https://github.com/studion79/studion-tasks_ynh/issues>

## Developer info

Please send your pull request to the [`testing` branch](https://github.com/studion79/studion-tasks_ynh/tree/testing).

To try the `testing` branch, please proceed like that:

```bash
sudo yunohost app install https://github.com/studion79/studion-tasks_ynh/tree/testing --debug
```

or

```bash
sudo yunohost app upgrade task_app -u https://github.com/studion79/studion-tasks_ynh/tree/testing --debug
```
