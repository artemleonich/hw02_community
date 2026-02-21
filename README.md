# Yatube — социальная сеть для публикации постов

[![CI](https://github.com/artemleonich/hw02_community/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/artemleonich/hw02_community/actions/workflows/python-app.yml)

Учебный проект курса Python-разработчик (Яндекс.Практикум).
Позволяет создавать посты, объединять их в тематические группы и просматривать ленту записей.

## Стек

- Python 3.7+
- Django 2.2

## Как запустить

```bash
# клонировать репо
git clone git@github.com:artemleonich/hw02_community.git
cd hw02_community

# создать и активировать виртуальное окружение
python3 -m venv venv
source venv/bin/activate

# установить зависимости
pip install -r requirements.txt

# применить миграции и запустить сервер
cd yatube
python manage.py migrate
python manage.py runserver
```

Проект будет доступен по адресу http://127.0.0.1:8000/
