# 🌟 Блогикум

**"Блогикум"** — это вебсайт для ведения блогов, построенный на фреймворке **Django**.

---

## 🛠️ Установка и настройка

### 1. Установите Python
Скачайте и установите последнюю версию Python с официального сайта: [python.org](https://www.python.org/).

### 2. Создайте виртуальное окружение и установите зависимости
Выполните следующие команды в терминале:
```sh
# Создать виртуальное окружение
python -m venv .venv

# Активировать окружение
source .venv/bin/activate  # Для Linux/MacOS
.venv\Scripts\Activate.ps1 # Для Windows

# Установить зависимости
pip install -r requirements.txt
```

### 3. Настройте базу данных
- Откройте файл settings.py в директории blogicum.
- Измените настройки базы данных, если вы не хотите использовать SQLite3.
- Примените миграции:
```sh
cd blogicum
python manage.py makemigrations
python manage.py migrate
```

### 4. Загрузите данные
Загрузите тестовые данные или свои собственные:
```sh
python manage.py loaddata db.json
```
### 5. Создайте суперпользователя
```sh
python manage.py createsuperuser
```

## ▶️ Запуск проекта
Запустите сервер разработки:
```sh
python manage.py runserver
```
Перейдите в браузере по адресу http://localhost:8000/.
**Админ-панель** доступна по адресу http://localhost:8000/admin/.