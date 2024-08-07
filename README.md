# Описание проекта «API для Yatube»
Проект API для социальной сети Yatube

# Установка
Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram.git
```

```
cd kittygram
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv venv
```

```
source venv/bin/activate
```

Установить зависимости из файла requirements.txt:

```
python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```

# Примеры запросов к API
POST ```/api/v1/jwt/create/```: Получить токен аутентификации. Отправьте свои username и password.
GET /api/v1/posts/: Получить список всех постов.
POST /api/v1/posts/: Создать новый пост.
GET /api/v1/posts/{post_id}/: Получить подробную информацию о посте.
PUT /api/v1/posts/{post_id}/: Полностью обновить пост.
PATCH /api/v1/posts/{post_id}/: Частично обновить пост.
DELETE /api/v1/posts/{post_id}/: Удалить пост.
GET /api/v1/groups/: Получить список всех групп.
GET /api/v1/groups/{group_id}/: Получить информацию о группе.
GET /api/v1/posts/{post_id}/comments/: Получить список всех комментариев к посту.
POST /api/v1/posts/{post_id}/comments/: Создать новый комментарий к посту.
GET /api/v1/posts/{post_id}/comments/{comment_id}/: Получить информацию о комментарии.
PUT /api/v1/posts/{post_id}/comments/{comment_id}/: Полностью обновить комментарий.
PATCH /api/v1/posts/{post_id}/comments/{comment_id}/: Частично обновить комментарий.
DELETE /api/v1/posts/{post_id}/comments/{comment_id}/: Удалить комментарий.
GET /api/v1/follow/: Получить подписчиков текущего пользователя.
POST /api/v1/follow/: Подписаться на пользователя.
