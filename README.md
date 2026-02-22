# hw02_community — Yatube

**[Русский](#русский) | [English](#english)**

---

## Русский

### Описание

Учебный проект — социальная платформа для публикации постов. Реализованы сообщества (группы), в которые пользователи могут объединять свои записи по тематикам. Проект создан в рамках курса Python-разработчик от Яндекс Практикума.

### Возможности

- Просмотр ленты всех постов на главной странице
- Группировка постов по тематическим сообществам
- Страница сообщества с фильтрацией постов по группе
- Админ-зона Django для управления контентом

### Технологии

- Python 3.7+
- Django 2.2.9
- SQLite
- pytest

### Структура проекта

```
hw02_community/
├── yatube/
│   ├── posts/          # Приложение постов и сообществ
│   │   ├── models.py   # Модели Post и Group
│   │   ├── views.py    # Представления (главная, страница группы)
│   │   ├── urls.py     # Маршруты приложения
│   │   └── admin.py    # Настройка админ-панели
│   ├── templates/      # HTML-шаблоны
│   ├── static/         # Статические файлы
│   └── yatube/         # Настройки проекта
├── tests/              # Автотесты
├── requirements.txt
└── README.md
```

### Запуск проекта

Клонируйте репозиторий:

```bash
git clone https://github.com/artemleonich/hw02_community.git
cd hw02_community
```

Создайте и активируйте виртуальное окружение:

```bash
python3 -m venv venv
source venv/bin/activate
```

Установите зависимости:

```bash
pip install -r requirements.txt
```

Выполните миграции:

```bash
cd yatube
python3 manage.py migrate
```

Запустите сервер разработки:

```bash
python3 manage.py runserver
```

Проект будет доступен по адресу http://127.0.0.1:8000/

### Запуск тестов

```bash
pytest
```

### Автор

Артём — [GitHub](https://github.com/artemleonich)

---

## English

### Description

A learning project — a social platform for publishing posts. Features thematic communities (groups) that allow users to organize their posts by topic. Built as part of the Yandex Practicum Python Developer course.

### Features

- View a feed of all posts on the main page
- Group posts by thematic communities
- Community page with posts filtered by group
- Django admin panel for content management

### Tech Stack

- Python 3.7+
- Django 2.2.9
- SQLite
- pytest

### Project Structure

```
hw02_community/
├── yatube/
│   ├── posts/          # Posts and communities app
│   │   ├── models.py   # Post and Group models
│   │   ├── views.py    # Views (index, group page)
│   │   ├── urls.py     # URL routing
│   │   └── admin.py    # Admin panel configuration
│   ├── templates/      # HTML templates
│   ├── static/         # Static files
│   └── yatube/         # Project settings
├── tests/              # Automated tests
├── requirements.txt
└── README.md
```

### Getting Started

Clone the repository:

```bash
git clone https://github.com/artemleonich/hw02_community.git
cd hw02_community
```

Create and activate a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run migrations:

```bash
cd yatube
python3 manage.py migrate
```

Start the development server:

```bash
python3 manage.py runserver
```

The project will be available at http://127.0.0.1:8000/

### Running Tests

```bash
pytest
```

### Author

Artem — [GitHub](https://github.com/artemleonich)
