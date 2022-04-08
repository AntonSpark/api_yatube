# api_yatube
#Авторский API для проекта Yatube 


## Описание
API учебного проекта Yatube, построенный на  Django REST Framework.

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:
```
git clone git@github.com:AntonSpark/api_yatube.git
```
Нужно создать и активировать виртуальное окружение:
```
python3 -m venv venv
```
```
source venv/Scripts/activate
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:
```
python manage.py migrate
```

Запустить проект:
```
python manage.py runserver
```

Далее все запросы производятся в програме Postman
Возможные Api запросы:
```
/api-token-auth/ (POST): передаём логин и пароль, получаем токен
```
```
/posts/ (GET, POST): получаем список постов или создаём пост
```
```
/posts/{post_id}/ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем пост по id
```
```
/groups/ (GET): получаем список групп
```
```
/groups/{group_id}/ (GET): получаем информацию о группе по id
```
```
/posts/{post_id}/comments/ (GET, POST): получаем список комментариев поста с id=post_id или создаём новый, указав id поста, который хотим прокомментировать
```
```
/posts/{post_id}/comments/{comment_id}/ (GET, PUT, PATCH, DELETE): получаем, редактируем или удаляем комментарий по id
```

## Автор
Anton Iskrov