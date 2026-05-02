# React + Docker — Hello, Docker!

Простое React-приложение, которое выводит "Hello, Docker!". Упаковано в Docker-образ с многоступенчатой сборкой.

## Скриншот

![Скриншот приложения](screenshot.png)

## Сборка и запуск

### 1. Собрать Docker-образ

```bash
docker build -t my-react-app .
2. Запустить контейнер
bash
docker run -d -p 8080:80 --name my-app-container my-react-app
3. Открыть в браузере
text
http://localhost:8080
4. Остановить и удалить контейнер
bash
docker stop my-app-container
docker rm my-app-container
Структура проекта
text
my-react-app/
├── src/
│   └── App.js
├── public/
│   └── index.html
├── Dockerfile
├── nginx.conf
├── .dockerignore
├── package.json
└── README.md
Используемые технологии
Технология	Назначение
React	Frontend-библиотека
Node.js (alpine)	Сборка приложения
nginx (alpine)	Веб-сервер
Docker (multi-stage)	Контейнеризация
Выполнил
Студент: _________________

Группа: _________________

Дата: ___________________ 
