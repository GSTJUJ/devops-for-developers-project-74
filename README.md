### Hexlet tests and linter status:
[![Actions Status](https://github.com/GSTJUJ/devops-for-developers-project-74/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/GSTJUJ/devops-for-developers-project-74/actions)
test

![push](https://github.com/ТВОЙ_ЛОГИН/devops-for-developers-project-74/actions/workflows/push.yml/badge.svg)

DevOps for Developers Project 74




Описание

Учебный проект с использованием Docker и Docker Compose.

Приложение представляет собой веб-сервис (Fastify + PostgreSQL), который запускается в контейнерах и полностью конфигурируется через переменные окружения.

Требования
Перед запуском убедитесь, что у вас установлены:

Docker
Docker Compose
Установка
make install
Запуск приложения (разработка)
make dev

После запуска приложение будет доступно по адресу:
https://localhost
Запуск тестов
make test

Тесты выполняются внутри Docker-контейнера.

Сборка образа
make build
Docker Hub

gstjuju/devops-for-developers-project-74

Пример .env файла:
 DATABASE_HOST=db
 DATABASE_NAME=postgres
 DATABASE_USERNAME=postgres
 DATABASE_PASSWORD=password


Команды Makefile
 make install — установка зависимостей
 make dev — запуск в режиме разработки
 make test — запуск тестов
 make build — сборка Docker-образа

Особенности
 Используется PostgreSQL в Docker
 Приложение полностью контейнеризировано
 Конфигурация через переменные окружения (12-factor app)
 CI запускает тесты внутри Docker