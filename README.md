# 💫 ORBIT LAB

> Доступный веб-инструмент для моделирования и визуализации орбитальной динамики. Проект решает проблему разрыва между абстрактными формулами и реальным пониманием космического полёта. Пользователь может настраивать начальные условия (скорость, угол, массы 2–3 небесных тел) и мгновенно видеть рассчитанную траекторию.

Проект команды **Galaxy Forces** для Космического идеатона БРИКС.

**Цель проекта:** создать доступный инструмент для моделирования космических полётов, позволяющий исследовать влияние начальных условий на траекторию и проверять результаты расчётов.

![Django](https://img.shields.io/badge/django-5.2.7-092E20?logo=django)
![Python](https://img.shields.io/badge/python-3.10%2B-blue?logo=python)

## 🛠 Технологический стек

- **Backend:** Python 3, Django, SciPy, NumPy
- **Frontend:** HTML5, CSS3, JavaScript (Canvas 2D)
- **База данных:** SQLite

## 🚀 Быстрый старт

### 1. Клонирование репозитория

```bash
git clone https://github.com/DreySych/OrbitLab.git
cd OrbitLab
```

### 2. Создание и активация виртуального окружения

```bash
python -m venv venv
```

Для Windows:

```bash
venv\Scripts\activate
```

Для macOS / Linux:

```bash
source venv/bin/activate
```

В терминале слева должна появиться приписка `(venv)`.

### 3. Установка зависимостей

```bash
pip install -r requirements.txt
```

### 4. Подготовка базы данных (миграции)

```bash
python manage.py migrate
```

### 5. Создание администратора

```bash
python manage.py createsuperuser
```

### 6. Запуск сервера

```bash
python manage.py runserver
```

### 7. Проверка работы

Откройте браузер и перейдите по ссылкам:

- 🌍 Сайт: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
- ⚙️ Админка: [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/)

## 📂 Кто где работает (структура проекта)

- `orbit_lab/` — главные настройки Django.
- `simulator/` — наше основное приложение:
  - `physics.py` — формулы, SciPy, интеграторы.
  - `views.py` — бэкенд: API для связи с фронтендом.
  - `models.py` — БД: хранение сценариев.
  - `templates/` — фронтенд: HTML.
  - `static/` — фронтенд: CSS, JS, Canvas.
