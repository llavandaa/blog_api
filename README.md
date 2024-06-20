# Blog API REST

Это REST API для ведения блога, разработанное с использованием Flask. API предоставляет возможность создания, чтения, обновления и удаления постов, а также создания пользователей.

## Установка/Запуск

1. Клонировать репозиторий:

    ```bash
    git clone https://github.com/llavandaa/blog_api.git
    cd blog_api
    ```

2. Установить зависимости:

    ```bash
    pip install -r requirements.txt
    ```

3. Запустить приложение:

    ```bash
    flask run
    ```

## Использование

### Создание пользователя

- **URL:** `/api/users`
- **Метод:** POST
- **Тело запроса:** JSON

  ```json
  {
      "username": "exampleuser",
      "email": "user@example.com"
  }
  
### Создание поста

- **URL:** `/api/posts`

- **Метод:** POST

- **Тело запроса:** JSON

  ```json
  {
    "title": "Название поста",
    "content": "Содержание поста",
    "user_id": "exampleuser2"
  }
  ```

### Получение поста

- **URL:** `/api/posts/<post_id>`

- **Метод:** GET

### Обновление поста

- **URL:** `/api/posts/<post_id>`

- **Метод:** PUT

- **Тело запроса:** JSON

  ```json
  {
      "title": "Updated Post",
      "content": "This is an updated post."
  }
  ```

### Удаление поста

- **URL:** `/api/posts/<post_id>`

- **Метод:** DELETE
