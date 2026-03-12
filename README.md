# Ansible Docker Installation

Этот проект содержит Ansible-роль и плейбук для автоматической установки Docker и Docker Compose на серверы с Ubuntu.

## Цель

Показать навыки написания идемпотентных Ansible-ролей, управления переменными, использования хендлеров и структурирования проектов.

## Технологии

- Ansible
- Docker / Docker Compose
- Ubuntu 22.04
- Git
- Vagrant (для локального тестирования)

## Как использовать

### Предварительные требования

- Управляющая машина с установленным Ansible (>=2.9).
- Целевые серверы с Ubuntu 20.04/22.04 и доступом по SSH.
- (Опционально) Vagrant и VirtualBox для локального тестирования.

### Быстрый старт с Vagrant

1. Клонируйте репозиторий:

   ```bash
   git clone https://github.com/yourusername/ansible-docker-install.git
   cd ansible-docker-install
   ```
2. Запустите виртуальные машины:

   ```
   vagrant up
   ```
3. Запустите плейбук:

   ```
   ansible-playbook playbooks/install-docker.yml
   ```
4. Проверьте установку на одном из хостов:

```
vagrant ssh host1
docker --version
docker compose version
```
