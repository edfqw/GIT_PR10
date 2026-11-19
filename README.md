# 🚀 TaskManager Pro
> ***Эффективное управление проектами никогда не было таким простым.*** ~~Теперь с поддержкой темной темы!~~
> ![Автор проекта](git.png)


## 📸 О проекте

*Современный менеджер задач для командной разработки*


## 👨‍💻 О разработчике
| Параметр | Значение |
| :--- | :--- |
| **Разработчик** | Daniil |
| **Роль** | Backend-разработчик, Технический писатель |
| **Email** | developer@example.com |
| **Telegram** | [@giga_dev](https://t.me/giga_dev) |
| **Специализация** | Высоконагруженные системы, автоматизация |
| **Статус проекта** | Пет-проект для оптимизации рабочих процессов |	

## 💻 Системные требования
| Компонент | Минимальная версия | Рекомендуемая версия |
| :--- | :--- | :--- |
| Python | 3.10 | 3.12 |
| PostgreSQL | 14 | 16 |
| Redis | 6.2 | 7.0 |
| Git | 2.30 | 2.45 |

Для работы приложения необходим установленный Python 3.10+ и система управления базами данных PostgreSQL 14+.


1. Клонирование репозитория
```bash
git clone https://github.com/username/taskmanager-pro.git
cd taskmanager-pro
```

2. Создание виртуального окружения
```bash
python -m venv venv
source venv/bin/activate  # Для Linux/macOS
venv\Scripts\activate     # Для Windows
```
3. Установка зависимостей
```bash
Копировать
pip install -r requirements.txt
```
4. Настройка переменных окружения

```Скопируйте файл примера и заполните свои данные:

bash
cp .env.example .env

Содержимое .env:

env
DB_NAME=taskmanager_db
DB_USER=postgres
DB_PASS=your_strong_password
SECRET_KEY=your_super_secret_key
```
5. Миграции и запуск сервера
```bash
python manage.py migrate
python manage.py runserver

Приложение доступно по адресу http://127.0.0.1:8000.
```

## 📁 Структура проекта
```
taskmanager-pro/
├── core/                 # Настройки проекта и общие утилиты
├── tasks/                # Основное приложение (модели, вьюхи, API)
├── templates/            # HTML-шаблоны
├── static/               # Статические файлы (CSS, JS, изображения)
├── tests/                # Тесты приложения
├── manage.py
└── requirements.txt      # Зависимости Python
```

## 📊 Таблица API эндпоинтов
| Метод | URL | Описание | Статус |
|---|---|---|---|
| GET | `/api/tasks/` | Получить список всех задач | ✅ |
| POST | `/api/tasks/` | Создать новую задачу | ✅ |
| GET | `/api/tasks/{id}/` | Получить детальную информацию | ✅ |
| PUT | `/api/tasks/{id}/` | Обновить задачу | ✅ |
| DELETE | `/api/tasks/{id}/` | Удалить задачу | ⚠️ (В разработке) |

## 💻 Пример вставки кода (Функция фильтрации)

Пример реализации фильтрации задач по статусу на Python:

```python
def filter_tasks_by_status(tasks, status):
    """
    Фильтрует список задач по заданному статусу.
    :param tasks: List[Task] - список объектов задач
    :param status: str - статус ('new', 'in_progress', 'done')
    :return: List[Task] - отфильтрованный список
    """
    return [task for task in tasks if task.status == status]
```
# Использование
```
active_tasks = filter_tasks_by_status(all_tasks, 'in_progress')
```

## Авторы
**Billie Thompson** - *Initial work* 

### 📄 Лицензия

Этот проект распространяется под лицензией MIT. С подробностями можно ознакомиться в файле LICENSE.

## 🤝 Вклад в разработку
```Форкните репозиторий.
Создайте ветку для фичи: git checkout -b feature/AmazingFeature.
Зафиксируйте изменения: git commit -m 'Add some AmazingFeature'.
Отправьте ветку: git push origin feature/AmazingFeature.
Откройте Pull Request.
```
Спасибо за ваш интерес к TaskManager Pro! 🎉

## ⬅️ Вернуться в начало

</details>
