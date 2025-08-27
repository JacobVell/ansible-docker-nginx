# Ansible Playbook: Docker + Nginx + Simple App

Этот проект демонстрирует использование **Ansible** для автоматической установки **Docker**, **Nginx** и деплоя простого веб-приложения.

## 📂 Структура проекта
```
ansible-docker-nginx/
├── inventory.ini        # список серверов
├── playbook.yml         # главный playbook
├── roles/
│   ├── docker/          # установка Docker
│   ├── nginx/           # настройка Nginx
│   └── app/             # деплой приложения
├── group_vars/          # переменные
└── README.md            # описание проекта
```

## 🚀 Использование

1. Склонировать репозиторий:
   ```bash
   git clone https://github.com/YOUR_USERNAME/ansible-docker-nginx.git
   cd ansible-docker-nginx
   ```

2. Указать IP и пользователя сервера в `inventory.ini`.

3. Запустить playbook:
   ```bash
   ansible-playbook -i inventory.ini playbook.yml --ask-become-pass
   ```

4. Открыть в браузере `http://<server-ip>` и увидеть страницу:
   ```
   Hello from Ansible automated deployment!
   ```

