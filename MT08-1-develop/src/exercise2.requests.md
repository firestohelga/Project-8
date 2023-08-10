## Какой запрос(-ы) отправляется на сервер для получения списка типов товаров в шторке "Каталог"?

POST https://sbermegamarket.ru/api/mobile/v1/catalogService/catalog/menu

## Какой запрос(-ы) отправляется на сервер при использовании поиска товаров в каталоге?

При открытии поиска:

POST https://sbermegamarket.ru/api/mobile/v3/catalogService/catalog/searchSuggest

При отправке запроса: 

POST https://sbermegamarket.ru/api/mobile/v1/catalogService/catalog/search

POST https://sbermegamarket.ru/api/mobile/v1/catalogService/filters/search

## Какой запрос(-ы) отправляется на сервер при поиске региона или города в модалке выбора вашего региона?
Запрос на эндпоинт POST /api/mobile/v1/addressSuggestService/address/suggest

HTTP-метод:POST , Полный URL запроса: https://sbermegamarket.ru/api/mobile/v1/addressSuggestService/address/suggest