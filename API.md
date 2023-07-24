### Users/Login
#### Опис: процедура Отримання токена, який буде використано для всіх наступних запитів
#### Запит:
curl --location 'http://domen/webservice/WebserviceStandard/Users/Login' \
--header 'X-API-KEY: **Веб-сервіс -> Додатки -> Ключ**' \
--header 'X-ENCRYPTED: 0' \
--header 'Content-Type: application/json' \
--header 'Authorization: Basic на основі **Веб-сервіс -> Додатки -> Назва** та **Веб-серві -> Додатки -> Пароль**' \
--data-raw '{
    "userName": "**Веб-сервіс -> Користувачі -> Логін**",
    "password": "**Пароль обраного користувача**",
    "params": {
        "language": "pl-PL"
    }
}'


### any req
#### Опис: структура будь-якого запиту не залежно від методу буде такою
#### Запит:
curl --location --request GET 'http://domen/webservice/WebserviceStandard/Leads/Record/131' \
--header 'X-API-KEY: **Веб-сервіс -> Додатки -> Ключ**' \
--header 'X-TOKEN: **Отримали під час _Users/Login_** ' \
--header 'Content-Type: application/json' \
--header 'Authorization: Basic на основі ** Веб-серві -> Додатки -> Назва** та **Веб-серві -> Додатки -> Пароль**' 
