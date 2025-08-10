### Описание

- запрос данных в Request Системы 1 из Системы 2 по id объекта
- формирование JSON с объектами Системой 2 
- передача файла в Response
- использование JWT на этапе запроса данных

Возможные сообщения
- 200 ОК
- 401 Не авторизован
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