# Yatube · Сообщества

<a href=".github/assets/light/stack.svg#gh-light-mode-only"><img src=".github/assets/light/stack.svg" height="28" alt="Python · Django · Learning" /></a><a href=".github/assets/stack.svg#gh-dark-mode-only"><img src=".github/assets/stack.svg" height="28" alt="Python · Django · Learning" /></a>

Лента публикаций и тематические группы на Django.

**Учебный проект**  
[Русский](#about) · [English](#english) · [Профиль](https://github.com/artemleonich)

<a id="about"></a>

## О проекте

Учебный этап проекта Yatube из курса Python-разработчика [Яндекс Практикума](https://practicum.yandex.ru/). Основной фокус — модели публикаций и групп, ORM, представления и HTML-шаблоны.

- Главная страница с десятью последними публикациями.
- Страница группы с десятью последними записями этой группы.
- Связь публикации с автором и необязательной группой.
- Админ-панель Django для управления авторами, группами и публикациями.

Публикации и группы на этом этапе создаются через админ-панель. Веб-формы публикации появляются в [hw03_forms](https://github.com/artemleonich/hw03_forms).

## Запуск

```bash
git clone https://github.com/artemleonich/hw02_community.git
cd hw02_community
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python yatube/manage.py migrate
python yatube/manage.py createsuperuser
python yatube/manage.py runserver
```

В Windows PowerShell: `.venv\Scripts\Activate.ps1`.

Откройте [127.0.0.1:8000](http://127.0.0.1:8000/). Учётная запись суперпользователя нужна для [админ-панели](http://127.0.0.1:8000/admin/), где можно добавить группы и публикации.

## Проверка

Учебные проверки находятся в `tests/`.

```bash
python -m pytest
```

## Навигация по коду

| Путь | Назначение |
| --- | --- |
| [yatube/posts/](yatube/posts/) | Модели и представления |
| [yatube/templates/](yatube/templates/) | Шаблоны интерфейса |
| [yatube/yatube/settings.py](yatube/yatube/settings.py) | Настройки и SQLite |
| [tests/](tests/) | Учебные проверки |

Зависимости сохранены в учебных версиях из [requirements.txt](requirements.txt). Запуск на новых версиях Python может потребовать адаптации окружения.

<a id="english"></a>

<details>
<summary>English overview</summary>

A Yandex Practicum learning stage focused on Django models, ORM queries and templates. It shows the latest ten posts on the home page and on each group page; content is managed through Django admin. The later [hw03_forms](https://github.com/artemleonich/hw03_forms) stage adds web forms.

Install `requirements.txt` in a virtual environment, run `python yatube/manage.py migrate`, optionally create an admin account with `python yatube/manage.py createsuperuser`, and start `python yatube/manage.py runserver`. Run `python -m pytest` from the repository root. Dependencies are pinned to the original learning versions.

</details>

---

Автор: [Артём Леонов](https://github.com/artemleonich).

