# Описание.

Проект "YaMDb" собирает отзывы пользователей на различные произведения.

# Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:
```
git clone git@github.com:Xewus/api_yamdb.git
```
```
cd api_yamdb
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
# Примеры запросов к API.

Получение списка всех произведений
```
GET /api/v1/titles/
```
Получить список всех отзывов к определенному произведению по его id
```
GET /api/v1/titles/{title_id}/reviews/
```
Получить список всех комментариев к отзыву по id
```
GET /api/v1/titles/{title_id}/reviews/{review_id}/comments/
```

**The final project of the Yandex Practicum backend course**

Writers:

https://github.com/KaterinaSolovyeva  (/titles, README)

https://github.com/nu-shtosh  (/users, settings)

https://github.com/Xewus   (/reviews, /api)

