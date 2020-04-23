# api_final
Проект по реализации API

Создано с помощью Django REST Framework

Описание:
реализация API для социальной сети (сайт, на котором можно создать свою страницу, посмотреть все записи автора, подписаться на авторов и комментировать их записи).

Установка:
Для установки ПО необходимо установить зависимости

pip install -r requirement.txt

Доступные методы:
/api/v1/token/
метод: POST

/api/v1/token/refresh/
метод: POST

/api/v1/posts/
методы: GET, POST

/api/v1/posts/{id}/
методы: GET, PUT, PATCH, DEL

/api/v1/posts/{post_id}/comments/
методы: GET, POST

/api/v1/posts/{post_id}/comments/{comment_id}/
методы: GET, PUT, PATCH, DEL

/api/v1/follow/
методы: GET, POST

/api/v1group/
методы: GET, POST


Примеры:

import requests

api = 'http://localhost:8000/api/v1/posts/'
headers - {'Authorization': 'Bearer <токен>'}
request = requests.get(api,headers=headers)




 

