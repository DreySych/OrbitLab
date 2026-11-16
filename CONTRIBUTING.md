# CONTRIBUTING

## 🔀 Как предложить изменение (Merge Request)

1. Создайте ветку от `main` (учтите правила оформления веток ниже)
2. Сделайте небольшие и атомарные изменения
3. Добавьте тесты и/или обновите документацию, если меняете поведение
4. Перед Merge Request обновите `main`:

   ```bash
   git pull origin main
   ```

## 💻 Локально

```bash
# Клонируйте репозиторий
git clone https://github.com/DreySych/OrbitLab.git
cd OrbitLab

# Создайте виртуальное окружение
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate     # Windows

# Установите зависимости
pip install -r requirements.txt

# Примените миграции
python manage.py migrate

```

## 📝 Правила оформления коммитов

Используйте следующие префиксы для сообщений коммитов (на английском):

### `Add` — добавление нового функционала
Используйте, когда добавляете новый код, файлы или компоненты

**Примеры:**
- `Add main app`
- `Add index page template`
- `Add profile view function`

### `Fix` — исправление ошибок
Используйте для багфиксов и исправлений некорректного поведения

**Примеры:**
- `Fix models in main`
- `Fix comments page template`
- `Fix password_restore view function`

### `Update` — обновление/изменение существующего
Используйте для изменения или улучшения существующего функционала

**Примеры:**
- `Update README`
- `Update urls list`
- `Update index view function`

### `Remove` — удаление кода/функционала
Используйте, когда удаляете файлы, функции или компоненты

**Примеры:**
- `Remove login button from profile page`
- `Remove birth date field from main/models.py`

### `Refactor` — рефакторинг кода
Используйте для улучшения читаемости и структуры без изменения функциональности

**Примеры:**
- `Refactor complaints page template`
- `Refactor user authentication logic`

## 🌿 Правила оформления веток

### Формат

<тип>/<краткое-описание>

### Требования
- ✅ **Язык**: только английский
- ✅ **Разделитель**: дефис `-` (kebab-case)
- ✅ **Регистр**: только строчные буквы
- ✅ **Длина**: 2–5 слов, достаточно для понимания цели
- ✅ **Префикс**: `feature/`, `fix/` или другие (со слешем)

### Типы веток

| Префикс    | Назначение                           | Пример                        |
|------------|--------------------------------------|-------------------------------|
| `feature/` | Новая функциональность               | `feature/ai-search-cache`     |
| `fix/`     | Исправление бага                     | `fix/login-redirect-error`    |
| `refactor/`| Рефакторинг без изменения логики     | `refactor/user-model-cleanup` |
| `docs/`    | Обновление документации              | `docs/update-readme`          |
| `test/`    | Добавление или исправление тестов    | `test/add-api-coverage`       |

### Примеры

- feature/add-data-save-api
- fix/paramets-upload
- refactor/trajectory-model
- docs/contributing-guide
- test/coverage-improvement

## ✅ Требования к коду


- Используйте понятные имена переменных
- Не коммитьте секреты (используйте `.env`)

