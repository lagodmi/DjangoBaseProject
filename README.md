# НАЗВАНИЕ.
## Описание проекта:
- 
## Стек проекта:
- Python 3.9
- Django 3.2.3
- Django REST framework 3.12.4
- JavaScript
## Cсылка на развернутый проект:
- 
## Процесс запуска проекта (через docker compose):
### Какую версию развернуть:
- В случае развертывания проекта в производственной среде следует использовать docker-compose.production.yml.
- Для разработки, тестирования или демонстрации концепции docker-compose.yml.
### Запуск проекта:
- Клонируем репозиторий:
    ??????
- Создаем файл .env в корне проекта c параметрами указанными в .env.example:
    nano .env
- Выполняем запуск:
    docker compose -f docker-compose.yml up -d
- Заходим в интерактивный терминал backend и выполняем команды:
    - docker compose exec -it backend bash
        - python manage.py migrate
        - python manage.py loaddb
        - python manage.py collectstatic
        - cp -r /app/collected_static/. /backend_static/static/
- Проект доступен на:
    http://localhost:8000/
### Пример запросов:
- 
## Автор проекта:
