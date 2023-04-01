## crud-jwt-spring-boot-3

# Реализация безопасности с использованием Spring boot 3.0  и JSON Web Token
## Функции:
Регистрация пользователя и вход в систему с JWT-аутентификацией
Шифрование паролей с помощью BCrypt
Авторизация на основе ролей с помощью Spring Security
Индивидуальная обработка отказа в доступе
Механизм выхода


## Технологии
Spring Boot 3.0
Spring Security
JSON Web Tokens (JWT)
BCrypt
Gradle

### Для этого проекто нужно:

JDK 17+
Maven 3+

### что бы запустить, выполните следующее:

- клонировать этот репозиторий
- установите зависимости
проверить работоспособность можно на POSTMAN
http://localhost:8080/api/v1/auth/authenticate
http://localhost:8080/api/v1/auth/register
регистрация: выбираем POST HTTP запрос, Body, row, выбираем json вместо text(по умолчанию) и пишем следующий пример:
    "firstname": "example",
    "lastname": "example",
    "email": "example@gmail.com",
    "password": "example"
    
    копируем токен который он сгенерировал:
http://localhost:8080/api/v1/demo-controller
    Выбираем GET HTTP запрос, authorization выбираем Type -> bearer token вставляем токен и нажимаем SEND
    При успешной авторизации и правильности входа выйдет следующий результат.

"Hello from secured endpoint"
