В данном проекте выполнено тестирование API учебного сервиса Яндекс Самокат.

В файле helpers описаны запросы: на удаление курьера(delete), метод генерации данных с применением библиотеки Faker, создание курьера(post)

В файле variables описаны локаторы эндпоинтов(class Urls), перемененные с ожидаемыми ответами(class MessageText), словари с генерацией тестовых данных для параметризации(class Data).

Зависимости находятся в requirements.txt

В папке tests содержатся тесты: test_create_courier.py с тестами на отправку запросов для создание курьера(POST), 

test_create_order.py с тестами на отправку запросов для создания заказов с разными вариантами выбора цвета(POST), где используется параметризация,

test_login_courier.py с тестами на отправку запросов для авторизации курьера с разными тестовыми случаями(POST),

test_order_list.py с тестами на отправку запросов для получения списка заказов(GET).

В конце каждого теста выполняется удаление созданного курьера(DELETE) с применением метода delete_courier(где применимо).

В каждома тесте выполняется 2 assert на код и на получаемое тело сообщения.

Во всех методах и тестах используется подробный allure для описания действий и тестов.

# Sprint_7
