**REST API** для сайта “Доска объявлений”.

На сайте пользователи выкладывают товары, которые хотели бы продать.  
Основные возможности:  

• Авторизация;

• Получение/редактирование данных текущего пользователя;

• Поиск и сортировка товаров;

• Загружать/удалять изображение для товара;

• Создание/редактирование/удаление товара авторизованным пользователем.

Пользователь авторизуется, используя email + password. В случае, если пользователь вводит email, которого нет в системе, новый пользователь с 
указанными email и password должен быть создан, а пользователь — авторизован. В дальнейшем пользователь может авторизоваться с указанными данными 
под тем же профилем.

Идентификация пользователя происходит по токену, который передается в заголовках HTTP запросов (заголовок Authorization). Токен пользователя 
создается на основе email, который является уникальным.

СУБД - MySQL (ORM - Sequelize).

Routes - Express.js.

Перед запуском необходимо создать БД с именем из config. Это можно сделать через http://localhost/phpmyadmin, при установки Ampps (https://www.ampps.com/).   
  
Для запуска проекта - npm start.
