### Спецификация синхронизации атрибутов объектов между системами

- запрос данных в Request Системы 1 из Системы 2 по id объекта
- формирование JSON с объектами Системой 2 
- передача файла в Response
- использование JWT на этапе запроса данных

Возможные сообщения
- 200 ОК
- 401 Неавторизован
- 403 Нет доступа
- 503 Сервер не доступен

parameters объектов
- id - uuid
- name – string
- created – date
- activation – boolean
- number – int
- elems – array {id – uuid, name – string, count – int}

[Scheme](https://github.com/Therealsergios/API-specifications/blob/main/rest/restapispec.yaml)

### Спецификация сервиса авторизации и аутентификации

- регистрация по номеру телефона
- подтверждение кода из SMS
- вход в систему
- выход из системы
- обновление токена
- получение и завершение сессий
- получение профиля пользователя

Возможные сообщения
- 204 Успешная авторизация
- 401 Неавторизован
- 404 Не найден

[Scheme](https://github.com/Therealsergios/API-specifications/blob/main/rest/auth.yaml)