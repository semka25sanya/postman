# postman
Регистрация:

Запрос:

https://blog.kata.academy/api/users
 {
  "user": {
    "username": "Alexa",
    "email": "semeenowa.alexandra@yandex.ru",
    "password": "semka25"
  }
}

Ответ: {"user":{"username":"alexa","email":"semeenowa.alexandra@yandex.ru","token":"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzZTJhYmVjNmY4YmVlMWIwMDU1MWUyYSIsInVzZXJuYW1lIjoiYWxleGEiLCJleHAiOjE2ODA5ODM1MzIsImlhdCI6MTY3NTc5OTUzMn0.-dvGPh1Qgv24Lx1Kz6Cbltab2ZYfI1LWeWR6L5jHrXs"}}

Авторизация:

Запрос:
https://blog.kata.academy/api/users/login
 {
  "user": {
    "email": "semeenowa.alexandra@yandex.ru",
    "password": "semka25"
  }
}
Ответ: {"user":{"username":"alexa","email":"semeenowa.alexandra@yandex.ru","token":"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzZTJhYmVjNmY4YmVlMWIwMDU1MWUyYSIsInVzZXJuYW1lIjoiYWxleGEiLCJleHAiOjE2ODA5ODQ5OTUsImlhdCI6MTY3NTgwMDk5NX0.RpqYgdyeM7VRe6sF9nXf-MmO0pjDo2b-Os1FH1EeKd4"}}

Берем токен, который получили при регистрации и делаем запрос по header

Ключ - Authorization:
Значение - Token eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzZTJhYmVjNmY4YmVlMWIwMDU1MWUyYSIsInVzZXJuYW1lIjoiYWxleGEiLCJleHAiOjE2ODA5ODQ5OTUsImlhdCI6MTY3NTgwMDk5NX0.RpqYgdyeM7VRe6sF9nXf-MmO0pjDo2b-Os1FH1EeKd4

Ответ: {"user":{"username":"alexa","email":"semeenowa.alexandra@yandex.ru","token":"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzZTJhYmVjNmY4YmVlMWIwMDU1MWUyYSIsInVzZXJuYW1lIjoiYWxleGEiLCJleHAiOjE2ODA5ODYxMzAsImlhdCI6MTY3NTgwMjEzMH0.HpowhnzzXBkW34bCN0r3xsaboGoIamwWEpWhP8MI6DA"}}
