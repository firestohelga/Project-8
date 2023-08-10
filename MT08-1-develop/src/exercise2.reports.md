# БАГ- РЕПОРТ

## Баг-репорт № 1. Код ответа 502 GET https://sbermegamarketru.webim.ru/button.php при обновлении главной страницы https://sbermegamarket.ru/


1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

- Нажать в браузере кнопку на обновить страницу


4. Ожидаемый результат:

- коды ответа у всех методов 200ые

5. Фактический результат:

- Код ответа 502 (Bad Gateway - Плохой шлюз)
- метод GET
- URL https://sbermegamarketru.webim.ru/button.php
- Заголовки запроса
```
Connection
	keep-alive
Content-Length
	1943
Content-Type
	text/html
Date
	Fri, 09 Jun 2023 07:24:59 GMT
ETag
	"6475134d-797"
Server
	nginx
```
- Заголовки ответа
```
Accept
	image/avif,image/webp,*/*
Accept-Encoding
	gzip, deflate, br
Accept-Language
	en-GB,en;q=0.5
Connection
	keep-alive
Host
	sbermegamarketru.webim.ru
Referer
	https://sbermegamarket.ru/
Sec-Fetch-Dest
	image
Sec-Fetch-Mode
	no-cors
Sec-Fetch-Site
	cross-site
User-Agent
	Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0
```
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at https://cms-res.online.sberbank.ru/sberid/BlackList/Button/No_Button.json. (Reason: CORS request did not succeed). Status code: (null).


6. Окружение: Windows 10 (Firefox, Версия 114.0 (64-bit))

## Баг-репорт № 2. При выботе региона Республика Татарстан г. Нижнекамск не открывается страница % МегаВыгода



1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Critical

3. Шаги для воспроизведения:

- Адрес доставки выбрать Республика Татарстан г. Нижнекамск
- Нажать на кнопку % МегаВыгода


4. Ожидаемый результат:

- страница открылась успешно, видны товары и т.д.

5. Фактический результат:

- Открывается страница, на которой написано 404 страница не найдена
- В DevTools выдает ошибку:

page url: /landing/discounter-msk/; message: Страница landing пустая; details: {"bannerCriteriaForLanding":{"startNum":300000101,"endNum":300000400,"slug":"discounter-msk","ignoringPlaces":["300000201","300000202","300000203","300000204","300000205","300000206","300000207","300000208","300000209","300000210","300000211","300000212","300000213","300000214","300000215","300000216","300000217","300000218","300000219","300000220","300000221","300000222","300000223","300000224","300000225","300000226","300000227","300000228","300000229","300000230","300000231","300000232","300000233","300000234","300000235","300000236","300000237","300000238","300000239","300000240","300000241","300000242","300000243","300000244","300000245","300000246","300000247","300000248","300000249","300000250","300000251","300000252","300000253","300000254","300000255","300000256","300000257","300000258","300000259","300000260","300000261","300000262","300000263","300000264","300000265","300000266","300000267","300000268","300000269","300000270","300000271","300000272","300000273","300000274","300000275","300000276","300000277","300000278","300000279","300000280","300000281","300000282","300000283","300000284","300000285","300000286","300000287","300000288","300000289","300000290","300000291","300000292","300000293","300000294","300000295","300000296","300000297","300000298","300000299","300000300"]},"banners":[]}


6. Окружение: Windows 10 (Firefox, Версия 114.0 (64-bit))

## Баг-репорт № 3. При выботе региона Республика Татарстан г. при нажатии кнопки "Подробнее" в в Push-уведомлении Войти по Сбер ID 



1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

- Адрес доставки выбрать Республика Татарстан г. Нижнекамск
- в Push-уведомлении Войти по Сбер ID нажать кнопку "Подробнее"


4. Ожидаемый результат:

- модальное окно открылось успешно, нет ошибок.

5. Фактический результат:

- модальное окно открылось
- В DevTools выдает ошибки:

Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at https://cms-res.online.sberbank.ru/sberid/BlackList/Button/No_Button.json. (Reason: CORS request did not succeed). Status code: (null).

GET https://cms-res.online.sberbank.ru/sberid/BlackList/Button/No_Button.json

[18:7:51:181] [info]  Ошибка получения чёрного списка.

6. Окружение: Windows 10 (Firefox, Версия 114.0 (64-bit))

## Баг-репорт № 4. При выботе региона Республика Татарстан г. Нижнекамск и отображании списока iphone 14 выдается ошибка



1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

- Адрес доставки выбрать Республика Татарстан г. Нижнекамск
- Нажать на строку поиска
- Из выпадающего списка "Часто ищут" выбрать iphone 14


4. Ожидаемый результат:

- отобразился список iphone 14, нет ошибок.

5. Фактический результат:

- отобразился список iphone 14
- В DevTools выдает ошибку:
```
TypeError: DDManager Custom Event "Viewed Campaign" Error

 t is null
    campaign https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    h https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    campaigns https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    h https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    enrichCommonData https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    enrichEventWithData https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    resolveHandlerAndFireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    trackImpression https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    setInterval handler*l/< https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    c https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    trackImpression https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    track https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    initialize https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    initialize https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    initialize https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    <anonymous> https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
node_modules.89ca50aa.js:2:383012
```


6. Окружение: Windows 10 (Firefox, Версия 114.0 (64-bit))

## Баг-репорт № 5. При выботе региона г. Москва и открытии корзина выдается ошибка



1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

- Адрес доставки выбрать г. Москва
- Добавить в корзину товар
- В левом верхнем углу нажать на значек корзина


4. Ожидаемый результат:

- Корзина успешно открылась, нет ошибок.

5. Фактический результат:

- Корзина открылась
- В DevTools выдает ошибки:
```
TypeError: DDManager Custom Event "Clicked ToCart Button (Desktop + Mobile Main Icon)" Error

 e.getAttribute(...) is null
    handler https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    run https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    resolveHandlerAndFireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    trackClick https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    i https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    o https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    trackClick https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    track https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    initialize https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    initialize https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    initialize https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    <anonymous> https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
node_modules.89ca50aa.js:2:383012
```
```
Uncaught ReferenceError: product is not defined
    <anonymous> https://sbermegamarket.ru/promo-page/letniy-zabeg-sladkie-radosti/ line 302 > injectedScript:1
    a https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:302
    b https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:303
    Qc https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:65
    e https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:205
    Ja https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:43
    q https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:206
    Yq https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:206
    vr https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:207
    Dr https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:211
    Ls https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:229
    Os https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:234
    push https://www.googletagmanager.com/gtm.js?id=GTM-WSJ2VMC:237
    push https://www.googletagmanager.com/gtag/js?id=DC-10810778&l=dataLayer&cx=c:255
    push https://www.googletagmanager.com/gtag/js:224
    push https://top-fwz1.mail.ru/js/code.js:32
    trackEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    pushEventQueue https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    o https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    _ https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireAddRemoveProduct https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    listenToEvents https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    H https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    J https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    updateItems https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    Ee https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    Re https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    n https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _wrapper https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    To https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    ht https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Lo https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    m https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    e https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    init https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
line 302 > injectedScript:1:156
```
``` 
TypeError: DDManager Custom Event "Viewed Campaign" Error

 t is null
    campaign https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    h https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    campaigns https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    h https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    enrichCommonData https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    enrichEventWithData https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    resolveHandlerAndFireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    trackImpression https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    setInterval handler*l/< https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    c https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    trackImpression https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    track https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    initialize https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    initialize https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    initialize https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    <anonymous> https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
node_modules.89ca50aa.js:2:383012
```
Uncaught (in promise) Timeout (i) 

6. Окружение: Windows 10 (Firefox, Версия 114.0 (64-bit))

## Баг-репорт № 6. При нажатии на картинку "Кэшбек до 60%" выдаются ошибки



1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

- Нажать на картинку "Кэшбек до 60%"

4. Ожидаемый результат:

- открылась страница https://sbermegamarket.ru/landing/cashback-na-pervyj-zakaz/, нет ошибок.

5. Фактический результат:

- открылась страница https://sbermegamarket.ru/landing/cashback-na-pervyj-zakaz/
- В DevTools выдает ошибки:
```
Uncaught ReferenceError: TouchEvent is not defined
    X https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    onTouchStart https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    n https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _wrapper https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    To https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    ht https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Lo https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    m https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    e https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    init https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    e https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    X https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    onTouchStart https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    n https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _wrapper https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    To https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    ht https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Lo https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    m https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    e https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    init https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    e https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
main.564c87f0.js:1:20029
```
```
Uncaught ReferenceError: TouchEvent is not defined
    X https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    onTouchStart https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    n https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _wrapper https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    To https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    ht https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Lo https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    m https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    e https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    init https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    e https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
main.564c87f0.js:1:20029
```
```
Uncaught ReferenceError: TouchEvent is not defined
    X https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    onTouchStart https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    n https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _wrapper https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    p https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    To https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    ht https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Lo https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    m https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    e https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    init https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    e https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
main.564c87f0.js:1:20029
```
```
TypeError: DDManager Custom Event "Viewed Campaign" Error

 t is null
    campaign https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    h https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    campaigns https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    h https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    enrichCommonData https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    enrichEventWithData https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    resolveHandlerAndFireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    trackImpression https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
node_modules.89ca50aa.js:2:383012
```

6. Окружение: Windows 10 (Firefox, Версия 114.0 (64-bit))

## Баг-репорт № 7. При нажатии на кнопку "Стать продавцом"

1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

- В правом верхнем углу нажать на кнопку "Стать продавцом"

4. Ожидаемый результат:

- Открылась страница https://sbermegamarket.ru/info/partners/, нет ошибок.

5. Фактический результат:

- Открылась страница https://sbermegamarket.ru/info/partners/
- В DevTools выдаются слебующие ошибки:
- POST https://sentry-dsn-customers.megamarket.tech/api/6/envelope/?sentry_key=6d82cc11d08a4657a9092ff80b4bd615&sentry_version=7
- Код ответа 503 (Service Unavailable - Служба недоступна)
- Заголовки запроса
```
access-control-allow-origin
	https://sbermegamarket.ru
access-control-expose-headers
	x-sentry-error, x-sentry-rate-limits, retry-after
Connection
	keep-alive
Content-Length
	84
Content-Type
	application/json
Date
	Fri, 09 Jun 2023 16:04:56 GMT
Server
	nginx
Strict-Transport-Security
	max-age=31536000; includeSubDomains
vary
	Origin
```
- Тело запроса:
```
{}

{"type":"client_report"}

{"timestamp":1686326695.954,"discarded_events":[{"reason":"sample_rate","category":"error","quantity":4}]}
```

- Заголовки ответа:
```
Accept
	*/*
Accept-Encoding
	gzip, deflate, br
Accept-Language
	en-GB,en;q=0.5
Connection
	keep-alive
Content-Length
	134
Content-Type
	text/plain;charset=UTF-8
Host
	sentry-dsn-customers.megamarket.tech
Origin
	https://sbermegamarket.ru
Referer
	https://sbermegamarket.ru/
Sec-Fetch-Dest
	empty
Sec-Fetch-Mode
	no-cors
Sec-Fetch-Site
	cross-site
User-Agent
	Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0
```
- Тело ответа: 

{"detail":"failed to queue envelope","causes":["envelope buffer capacity exceeded"]}

```
Uncaught TypeError: e.$slides is null
    <anonymous> https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:64
    dispatch https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:39
    handle https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:39
    trigger https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:39
    trigger https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:39
    each https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:28
    each https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:28
    trigger https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:39
    init https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:39
    e https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:39
    slick https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:39
    <anonymous> https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:64
    n https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:1
    <anonymous> https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:1
    <anonymous> https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/mobile/js/desktop.js:1
desktop.js:64:60839
```
```
TypeError: DDManager Custom Event "Viewed Product Listing" Error

 t.digitalData(...) is undefined
    handler https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    run https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    resolveHandlerAndFireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    trackEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireUnfiredEvents https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireUnfiredEvents https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    H https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    $ https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    te https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    setLocationInfo https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    fetchCurrentLocation https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    fetchLocationData https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    identifyRegion https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    mounted https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    zn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    insert https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    E https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    e https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    52038 https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    transitionTo https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    transitionTo https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    confirmTransition https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Ce https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    confirmTransition https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    c https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Re https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    promise callback*Me/</< https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    je https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    je https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    je https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Me https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Ce https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    confirmTransition https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    transitionTo https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    init https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    beforeCreate https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    zn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _init https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Lr https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xa https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    52038 https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    d https://extra-cdn.sbermegamarket.ru/static/dist/rtm.ee00827d.js:1
    <anonymous> https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    O https://extra-cdn.sbermegamarket.ru/static/dist/rtm.ee00827d.js:1
    <anonymous> https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    a https://extra-cdn.sbermegamarket.ru/static/dist/rtm.ee00827d.js:1
    <anonymous> https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
node_modules.89ca50aa.js:2:383012
```
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at https://cms-res.online.sberbank.ru/sberid/BlackList/Button/No_Button.json. (Reason: CORS request did not succeed). Status code: (null).

ross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-1421183-77G99&products_event=view_other&price_list_id=1&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error node_modules.89ca50aa.js:2:383012
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-1522272-gSw6t&products_event=view_other&price_list_id=1&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error node_modules.89ca50aa.js:2:383012
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-1392950-ns48&products_event=view_other&price_list_id=1&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error node_modules.89ca50aa.js:2:383012
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-740345-e0KWW&products_event=view_other&price_list_id=1&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error node_modules.89ca50aa.js:2:383012
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-934121-8M7uZ&products_event=view_other&price_list_id=1&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error

Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-1042270-gnJEy&products_event=view_other&price_list_id=140664&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error node_modules.89ca50aa.js:2:383012
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-1042270-gnJEy&products_event=view_other&price_list_id=343775&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error node_modules.89ca50aa.js:2:383012
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-1042270-gnJEy&products_event=view_other&price_list_id=352574&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error node_modules.89ca50aa.js:2:383012
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-1042270-gnJEy&products_event=view_other&price_list_id=343768&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error node_modules.89ca50aa.js:2:383012
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-1042270-gnJEy&products_event=view_other&price_list_id=343764&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error node_modules.89ca50aa.js:2:383012
Cross-Origin Request Blocked: The Same Origin Policy disallows reading the remote resource at ‘https://vk.com/rtrg?p=VK-RTRG-1042270-gnJEy&products_event=view_other&price_list_id=343773&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fpartners%2F&metatag_title=%D0%A1%D0%B1%D0%B5%D1%80%D0%9C%D0%B5%D0%B3%D0%B0%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%20-%20%D0%BF%D0%B0%D1%80%D1%82%D0%BD%D1%91%D1%80%D0%B0%D0%BC%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru’. (Reason: Credential is not supported if the CORS header ‘Access-Control-Allow-Origin’ is ‘*’).

Open api access error

```
Uncaught (in promise) TypeError: e is null
    getSize https://yastatic.net/s3/front-maps-static/maps-front-jsapi-v2-1/2.1.79-11532562/build/release/full-2e211ea3bc39b6696fa8e65a7c24d6a38733cebe.js:1420
    v https://yastatic.net/s3/front-maps-static/maps-front-jsapi-v2-1/2.1.79-11532562/build/release/full-2e211ea3bc39b6696fa8e65a7c24d6a38733cebe.js:606
    J https://yastatic.net/s3/front-maps-static/maps-front-jsapi-v2-1/2.1.79-11532562/build/release/full-2e211ea3bc39b6696fa8e65a7c24d6a38733cebe.js:618
    <anonymous> https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/desktop/js/desktop.js:64
    promise callback* https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/desktop/js/desktop.js:64
    n https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/desktop/js/desktop.js:1
    <anonymous> https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/desktop/js/desktop.js:1
    <anonymous> https://main-cdn.sbermegamarket.ru/upload/static_pages/1/d1/457/1d1457c9c6321a015e901d04146b0ffb/desktop/js/desktop.js:1
full-2e211ea3bc39b6696fa8e65a7c24d6a38733cebe.js:1420:3317
```


6. Окружение: Windows 10 (Firefox, Версия 114.0 (64-bit))


## Баг-репорт № 8. Ошибка при нажатии на кнопку "Скидки до 50% на товары для животных" 

1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

- Нажать на кнопку "Скидки до 50% на товары для животных" рассположенную по середине страницы. 
- После открытия страницы, в панели справа выбрать чек-бокс "Brit" в вкладке "Бренды".


4. Ожидаемый результат:

- Откроется новая страница с товарами для животных бренда "Brit" без наличия ошибок в DevTools.

5. Фактический результат:

- Страница открыта, товары отображаются. 
- Вышла ошибка:
```
message: Multiple popovers with the same name detected; details: {"popoverName":"CatalogItemCreditPopover-100001284143/40441/","stack":"_registerPopover@https://extra-cdn.sbermegamarket.ru/static/dist/plugins.42c5f131.js:1:16631\nsetup/<@https://extra-cdn.sbermegamarket.ru/static/dist/plugins.42c5f131.js:1:52064\nasync*nn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:536759\nzn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:542500\ninsert@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:546239\nE@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:581518\n20144/xi</<@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:582877\n20144/</e.prototype._update@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:558792\nr@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:589761\n20144/Tn</e.prototype.get@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:540297\n20144/Tn</e.prototype.run@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:541030\ner@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:542996\nvn/<@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:537828\nln@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:537227\npromise callback*sn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:537317\nvn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:537891\ntr@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:543614\n20144/Tn</e.prototype.update@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:540966\n20144/we</e.prototype.notify@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:522899\nset@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:524702\nTt@https://extra-cdn.sbermegamarket.ru/static/dist/3298.b9af6150.js:1:11543\nasync*setup/<@https://extra-cdn.sbermegamarket.ru/static/dist/3298.b9af6150.js:1:14415\nnn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:536759\nzn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:542500\ninsert@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:546239\nE@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:581518\n20144/xi</<@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:582877\n20144/</e.prototype._update@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:558792\nr@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:589761\n20144/Tn</e.prototype.get@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:540297\n20144/Tn</e.prototype.run@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:541030\ner@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:542996\nvn/<@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:537828\nln@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:537227\npromise callback*sn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:537317\nvn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:537891\ntr@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:543614\n20144/Tn</e.prototype.update@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:540966\n20144/we</e.prototype.notify@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:522899\nset@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:524702\nm@https://extra-cdn.sbermegamarket.ru/static/dist/9621.4ea9f012.js:1:311\nl@https://extra-cdn.sbermegamarket.ru/static/dist/9621.4ea9f012.js:1:417\nasync*v/</<@https://extra-cdn.sbermegamarket.ru/static/dist/9621.4ea9f012.js:1:2842\nnn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:536759\nzn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:542500\n20144/Lr.prototype.$mount/<@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:589726\n20144/Lr.prototype.$mount@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:590003\ninit@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:545199\nn@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:549036\nd/<@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:577863\nd@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:578140\nk/<@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:580991\nk@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:581175\nk/<@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:580700\nk@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:581175\nk/<@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:580700\nk@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:581175\n20144/xi</<@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:582311\n20144/</e.prototype._update@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:558792\nr@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:589761\n20144/Tn</e.prototype.get@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:540297\n20144/Tn</e.prototype.run@https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2:541030\n"} node_modules.89ca50aa.js:2:383012
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    error https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    error https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    errorFormatted https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    handleError https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
    _registerPopover https://extra-cdn.sbermegamarket.ru/static/dist/plugins.42c5f131.js:1
    setup https://extra-cdn.sbermegamarket.ru/static/dist/plugins.42c5f131.js:1
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    zn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    insert https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    E https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    run https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    er https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    vn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    ln https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    (Асинхронный: promise callback)
    sn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    vn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    tr https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    notify https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    set https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    Tt https://extra-cdn.sbermegamarket.ru/static/dist/3298.b9af6150.js:1
    setup https://extra-cdn.sbermegamarket.ru/static/dist/3298.b9af6150.js:1
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    zn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    insert https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    E https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    run https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    er https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    vn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    ln https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    (Асинхронный: promise callback)
    sn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    vn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    tr https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    notify https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    set https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    m https://extra-cdn.sbermegamarket.ru/static/dist/9621.4ea9f012.js:1
    l https://extra-cdn.sbermegamarket.ru/static/dist/9621.4ea9f012.js:1
    v https://extra-cdn.sbermegamarket.ru/static/dist/9621.4ea9f012.js:1
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    zn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    $mount https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    init https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    n https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    k https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    k https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    k https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    k https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    k https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    k https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    xi https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    _update https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    r https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    get https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
    run https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
```
6. Окружение: Windows 11 (Firefox, Версия 114.0 (64-bit))

## Баг-репорт № 9. Ошибка при нажатии на кнопку "Продукты питания"

1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

-  Нажать на кнопку "Продукты питания" рассположенную в блоке "Категории товаров" в низу страницы. 

4. Ожидаемый результат:

- страница открылась успешно, товары отображаются, без наличия ошибок в DevTools.

5. Фактический результат:

- страница открылась успешно, товары отображаются, в DevTools отображенна ошибка;

```
TypeError: DDManager Custom Event "Viewed Campaign" Error

 t is null
    campaign https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    h https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    campaigns https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    h https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    enrichCommonData https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    enrichEventWithData https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    resolveHandlerAndFireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    trackImpression https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    a https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
node_modules.89ca50aa.js:2:383012
```


6. Окружение: Windows 10 (Firefox, Версия 114.0 (64-bit))


## Баг-репорт № 10. Код ответа 400 GET GET https://online.sberbank.ru/CSAFront/api/oidc/sbidclient_id=52cd75e2-76e1-43ba-ade6-938b2c7d4e7a при переключении вкладок. 


1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

- Нажать на кнопку "Одежда, Обувь, Аксессуары" рассположенную в блоке "Категории товаров" в низу страницы. 


4. Ожидаемый результат:

- коды ответа у всех методов 200ые

5. Фактический результат:

- Код ответа 400 (400 Bad Request)
- метод GET
- URL https://online.sberbank.ru/CSAFront/api/oidc/sbid?client_id=52cd75e2-76e1-43ba-ade6-938b2c7d4e7a
- Заголовки запроса
```
Accept: */*
Accept-Encoding: gzip, deflate, br
Accept-Language: ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3
Connection:	keep-alive
Cookie:
	f5avraaaaaaaaaaaaaaaa_session_=GDGKKIDNOPIGHHFNFJJGDLGPBDIJOIMIMBFKGBHKPMELEOMOIEDPDFEGCLIEGGLHAEGDNJCAPGOLEPFHIBBAMJGNNJKFOBFICKKCCNIJDHOHEGHCGCAADDEABNNECDFA; ESAWEBJSESSIONID=PBC5YS:1281246610; TS0135c014=0156c5c860c98ab37a23f1bb41db835a6068435d37c38a5639cb2692141c8ce64dff6d6f53c6236a2969e35e42a764d7643107ea5a5f64621dd7b4001c4b84587664e7a098; _sv=SA1.4f089e79-e702-454e-873f-c2721a9ae0d2.1686211456; _ym_isad=2; _ym_uid=1686317189293767511; _ym_d=1686332868; JSESSIONID=node01vjmbwbufkjebwrzfs5c8l71x41508770.node0; TS019e0e98=0156c5c860c50db473d73f9cf1984dfd7f8553d1c45ee8744880cafc12b5a118f558e4e9d266ad1fcda8336139c0fb7afa1fc50d1e54e2b74a4373917411a39cf835a0dffcf783119d0b9812897429118cc8584f7eb2cf77fdb6caeb3532665bbe74373a50206033aeb96299659d393d4bc0caf22a; TS3bb85bd7027=08bd9624b8ab200025008f0bf6997a4cf2df3d914ee268b741cabb27c6cfabae14ec44317a0ceaf108a0c3f50b113000bd420f20e88438778167675bc6e49d45a5ee2629ff0eab2a4f85f7cb9e19a16b5a9f70ee8b92e3cf7dadb43d659e1149
Host: online.sberbank.ru
Origin: https://sbermegamarket.ru
Referer: https://sbermegamarket.ru/
Sec-Fetch-Dest: empty
Sec-Fetch-Mode: cors
Sec-Fetch-Site: cross-site
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0
```
- Заголовки ответа
```
Access-Control-Allow-Credentials: true
Access-Control-Allow-Methods: GET
Access-Control-Allow-Origin: https://sbermegamarket.ru
Access-Control-Max-Age: 600
Connection: keep-alive
Content-Length: 0
Date: Fri, 09 Jun 2023 21:21:10 GMT
Set-Cookie:
TS3bb85bd7027=08bd9624b8ab2000d2b17d2a07dc478363f5ac6b147a27fb228506f0a47f97f8d35691122bf6cb7008febd7ec3113000a6964fc33c790b3608695d090b48d5cd1b8ca56c91e55126ce122429bf719383bdf6ed64b060a4b9d4f856a9de0e39eb; Path=/
```

6. Окружение: Windows 11 (Firefox, Версия 114.0 (64-bit))


## Баг-репорт № 11. Ошибка при нажатиина кнопку при переключении вкладок на странице https://sbermegamarket.ru/catalog/odezhda-obuv-i-aksessuary/

1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

-  Нажать на кнопку "Одежда, Обувь, Аксессуары" рассположенную в блоке "Категории товаров" в низу страницы. 
- Откроется страница "https://sbermegamarket.ru/catalog/odezhda-obuv-i-aksessuary/"
- Обновить страницу.

4. Ожидаемый результат:

- страница открылась успешно, товары отображаются, без наличия ошибок в DevTools.

5. Фактический результат:

- страница открылась успешно, товары отображаются, в DevTools отображенна ошибка;

```
Open api access error 11 node_modules.89ca50aa.js:2:383012
v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
onerror https://vk.com/js/api/openapi.js?169:672
s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
(Асинхронный: EventHandlerNonNull)
u https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
makeRequest https://vk.com/js/api/openapi.js?169:678
ProductEvent https://vk.com/js/api/openapi.js?169:3137
onViewedOther https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
onViewedOther https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
onViewedOther https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
onViewedPage https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
(Асинхронный: setTimeout handler)
l https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
onViewedPage https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
trackEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
pushEventQueue https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
o https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
fireUnfiredEvents https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
fireUnfiredEvents https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
H https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
$ https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
te https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
setLocationInfo https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
fetchCurrentLocation https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
fetchLocationData https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
identifyRegion https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
mounted https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0.js:1
nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
zn https://extra-cdn.sbermegamarket.rustatic/dist/node_modules.89ca50aa.js:2
insert https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.89ca50aa.js:2
```

6. Окружение: Windows 11 (Firefox, Версия 114.0 (64-bit))


## Баг-репорт № 12. Ошибка при нажатии на кнопку "Возвращать товары легко" https://sbermegamarket.ru/info/legkie-vozvraty/ 

1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Открыт DevTools


2. Серьезность: Minor

3. Шаги для воспроизведения:

-  Нажать на кнопку "Возвращать товары легко" рассположенную под блоком "Популярные товары Самокат" в низу страницы. 
- Откроется страница https://sbermegamarket.ru/info/legkie-vozvraty/

4. Ожидаемый результат:

- страница открылась успешно, изображения отображаются, без наличия ошибок в DevTools.

5. Фактический результат:

- страница открылась успешно, изображения  отображаются, в DevTools отображенна ошибка;

```
Запрос из постороннего источника заблокирован: Политика одного источника запрещает чтение удаленного ресурса на «https://vk.com/rtrg?p=VK-RTRG-1421183-77G99&products_event=view_other&price_list_id=1&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Flegkie-vozvraty%2F&metatag_title=%D0%9B%D0%B5%D0%B3%D0%BA%D0%B8%D0%B5%20%D0%B2%D0%BE%D0%B7%D0%B2%D1%80%D0%B0%D1%82%D1%8B%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru». (Причина: Учётные данные не поддерживаются, если заголовок CORS «Access-Control-Allow-Origin» установлен в «*»).
```

6. Окружение: Windows 11 (Firefox, Версия 114.0 (64-bit))

## Баг-репорт № 13. Код ответа 404 GET https://sbermegamarket.ru/info/about-sbermegamarket-ru/desktop/css/desktop.css при переходе в раздел "О компании"  https://sbermegamarket.ru/info/about-sbermegamarket-ru/


1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Запущен DevTools браузера вкладка "Консоль".


2. Серьезность: Minor

3. Шаги для воспроизведения:

- В футере главной странице нажать на раздел "О компании"


4. Ожидаемый результат:

- коды ответа у всех методов 200ые

5. Фактический результат:

- Код ответа 404 Not Found
- метод GET
- URL https://sbermegamarket.ru/info/about-sbermegamarket-ru/desktop/css/desktop.css
- Заголовки запроса
```
Accept
	text/css,*/*;q=0.1
Accept-Encoding
	gzip, deflate, br
Accept-Language
	ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3
Connection
	keep-alive
Cookie
	spid=1686423885155_82303fc297ca6c954dc7367208fdb4ea_qxaoxw96kcihpcb7; spsc=1686423885155_de6c0948da039c8ebdbaf02b2d5cbbf9_a5476469b72f558bb72e6aae99c6a060; oxxfgh=eee855cf-be23-4766-ba38-6d72d2f97b1b#1#7776000000#5000#1800000; KFP_DID=fa3ef900-ea7f-b943-7217-1ab7fc7d120d; adspire_uid=AS.1063465999.1686423823; ssaid=852dfc10-07c1-11ee-9a1d-25e47a2dc316; device_id=ab8964b3-07c1-11ee-9174-0242ac110004; sbermegamarket_token=1edb6efd-5039-46e3-8e93-a109cf35a9e7; cfidsw-smm=OVtKmva7fORdyj8+Y0gQoVRwGJ1CBxqvzlVDPxt…D0%BB%D0%B0%D1%81%D1%82%D1%8C%22%2C%22kladrId%22%3A%225000000000000%22%2C%22isDeliveryEnabled%22%3Atrue%2C%22geo%22%3A%7B%22lat%22%3A55.755814%2C%22lon%22%3A37.617635%7D%2C%22id%22%3A%2250%22%7D; _sa=SA1.6e413a3d-e30e-4481-96ee-3eea7d4361b9.1686423828; rrpvid=139247007372132; _gcl_au=1.1.1989232289.1686423829; uxs_uid=8886c400-07c1-11ee-9902-75569f49c94f; rcuid=6484c955a176af6d166c3fdf; _gpVisits={"isFirstVisitDomain":true,"idContainer":"10002472"}; _gp10002472={"hits":4,"vc":1,"ac":1,"a6":1}; __tld__=null
DNT
	1
Host
	sbermegamarket.ru
Referer
	https://sbermegamarket.ru/info/about-sbermegamarket-ru/
Sec-Fetch-Dest
	style
Sec-Fetch-Mode
	no-cors
Sec-Fetch-Site
	same-origin
TE
	trailers
User-Agent
	Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0
```
- Заголовки ответа
```
ontent-encoding
	gzip
content-type
	text/html
date
	Sat, 10 Jun 2023 19:22:19 GMT
server
	nginx
strict-transport-security
	max-age=31536000; includeSubDomains
X-Firefox-Spdy
	h2
x-sp-crid
	164389858:66
```

6. Окружение: Windows 11 Pro  (Firefox, Версия 114.0 (64-bit))

## Баг-репорт № 14. Код ответа 404 GET https://sbermegamarket.ru/info/about-sbermegamarket-ru/js/desktop.js при переходе в раздел "О компании"  https://sbermegamarket.ru/info/about-sbermegamarket-ru/


1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Запущен DevTools браузера вкладка "Консоль".


2. Серьезность: Minor

3. Шаги для воспроизведения:

- В футере главной странице нажать на раздел "О компании"


4. Ожидаемый результат:

- коды ответа у всех методов 200ые

5. Фактический результат:

- Код ответа 404 Not Found
- метод GET
- URL https://sbermegamarket.ru/info/about-sbermegamarket-ru/js/desktop.js
- Заголовки запроса
```
Accept
	*/*
Accept-Encoding
	gzip, deflate, br
Accept-Language
	ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3
Connection
	keep-alive
Cookie
	spid=1686423885155_82303fc297ca6c954dc7367208fdb4ea_qxaoxw96kcihpcb7; spsc=1686423885155_de6c0948da039c8ebdbaf02b2d5cbbf9_a5476469b72f558bb72e6aae99c6a060; oxxfgh=eee855cf-be23-4766-ba38-6d72d2f97b1b#1#7776000000#5000#1800000; KFP_DID=fa3ef900-ea7f-b943-7217-1ab7fc7d120d; adspire_uid=AS.1063465999.1686423823; ssaid=852dfc10-07c1-11ee-9a1d-25e47a2dc316; device_id=ab8964b3-07c1-11ee-9174-0242ac110004; sbermegamarket_token=1edb6efd-5039-46e3-8e93-a109cf35a9e7; cfidsw-smm=OVtKmva7fORdyj8+Y0gQoVRwGJ1CBxqvzlVDPxt…D0%BB%D0%B0%D1%81%D1%82%D1%8C%22%2C%22kladrId%22%3A%225000000000000%22%2C%22isDeliveryEnabled%22%3Atrue%2C%22geo%22%3A%7B%22lat%22%3A55.755814%2C%22lon%22%3A37.617635%7D%2C%22id%22%3A%2250%22%7D; _sa=SA1.6e413a3d-e30e-4481-96ee-3eea7d4361b9.1686423828; rrpvid=139247007372132; _gcl_au=1.1.1989232289.1686423829; uxs_uid=8886c400-07c1-11ee-9902-75569f49c94f; rcuid=6484c955a176af6d166c3fdf; _gpVisits={"isFirstVisitDomain":true,"idContainer":"10002472"}; _gp10002472={"hits":4,"vc":1,"ac":1,"a6":1}; __tld__=null
DNT
	1
Host
	sbermegamarket.ru
Referer
	https://sbermegamarket.ru/info/about-sbermegamarket-ru/
Sec-Fetch-Dest
	script
Sec-Fetch-Mode
	no-cors
Sec-Fetch-Site
	same-origin
TE
	trailers
User-Agent
	Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0
```
- Заголовки ответа
```
content-encoding
	gzip
content-type
	text/html
date
	Sat, 10 Jun 2023 19:22:19 GMT
server
	nginx
strict-transport-security
	max-age=31536000; includeSubDomains
X-Firefox-Spdy
	h2
x-sp-crid
	164389858:67
```

6. Окружение: Windows 11 Pro  (Firefox, Версия 114.0 (64-bit))


## Баг-репорт № 15. Ошибка в разделе "О компании" https://sbermegamarket.ru/info/about-sbermegamarket-ru/
1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Запущен DevTools браузера вкладка "Консоль".


2. Серьезность: Minor

3. Шаги для воспроизведения:

 - В футере главной странице нажать на раздел "О компании"

4. Ожидаемый результат:

- страница открылась успешно, изображения отображаются, без наличия ошибок в DevTools.

5. Фактический результат:

- страница открылась успешно, изображения  отображаются, в DevTools отображена ошибка;

```
downloadable font: rejected by sanitizer (font-family: "Graphik LCG" style:normal weight:400 stretch:100 src index:0) source: https://main-cdn.sbermegamarket.ru/upload/static_pages/e/ab/738/eab738ad5e489ec2e334cf82dd047923/desktop/fonts/GraphikLCGRegular.eot
```

6. Окружение: Windows 11 Pro  (Firefox, Версия 114.0 (64-bit))

## Баг-репорт № 16. Ошибка в разделе " Реквизиты" https://sbermegamarket.ru/info/rekvizity/
1. Предшествующие условия

- Открыта страница https://sbermegamarket.ru/ в браузере Firefox
- Запущен DevTools браузера вкладка "Консоль".


2. Серьезность: Minor

3. Шаги для воспроизведения:

 - В футере главной странице нажать на раздел "Реквизиты"

4. Ожидаемый результат:

- страница открылась успешно, изображения отображаются, без наличия ошибок в DevTools.

5. Фактический результат:

- страница открылась успешно, изображения  отображаются, в DevTools отображена ошибка;

```
error loading "library" error="Error: script error "https://mc.yandex.ru/metrika/tag.js"" node_modules.89ca50aa.js:2:383012  

error loading "library" error="Error: script error "https://top-fwz1.mail.ru/js/code.js""  node_modules.89ca50aa.js:2:383012

error loading "library" error="Error: script error "https://api.flocktory.com/v2/loader.js?site_id=2319"" node_modules.89ca50aa.js:2:383012  

error loading "library" error="Error: script error "https://vk.com/js/api/openapi.js?150"" node_modules.89ca50aa.js:2:383012  

```

6. Окружение: Windows 11 Pro  (Firefox, Версия 114.0 (64-bit))



