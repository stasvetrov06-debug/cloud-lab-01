cat > README.md << 'EOF'
# Cloud Lab

## Назначение
Учебное REST API, разработанное в облачной среде GitHub Codespaces.
Демонстрирует работу с Node.js, Express, переменными окружения и конфигурацией devcontainer.

## Технологии
- Node.js 22
- Express
- GitHub Codespaces

## Установка
npm install

## Запуск
npm start

## Маршруты
| Метод | Маршрут | Описание |
|-------|---------|----------|
| GET | / | HTML-страница со ссылками |
| GET | /api/status | Состояние сервера (имя приложения, время, hostname) |
| GET | /api/hello | Приветствие; имя задаётся параметром ?name=, иначе «Гость» |
| GET | /api/services | Список всех сервисов |
| GET | /api/services/:id | Один сервис по идентификатору; 404 если не найден |
| POST | /api/services | Добавить сервис (поля name и category); 400 при пустых полях, 201 при успехе |
EOF