# Описание метатегов

## Тег `meta`

Принимает как минимум 4 атрибута: `content`, `http-equiv`, `name`, `scheme`.<br>
Из них обязателен только `content`.

Рассмотрим основные из них.

### Name `charset`

Определяет кодировку символов

Пример использования:

    <meta charset="UTF-8" />

### Name `viewport`

Принимает 5 параметров:

- `width` - определяет ширину области просмотра. Чаще всего принимает параметр `device-width`, что означает использовать всю доступную ширину экрана. Может также принимать значения от 1 до 10000;
- `height` - определяет высоту области просмотра;
- `initial-scale` - уровень масштабирования при первой загрузке странице. Доступны значения от 0.1 до 10.

Пример использования:

    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

### Name `application-name`

Указывется название веб-приложения, которое представляет данный сайт. Не должен использоваться если сайт не используется как веб-приложение.

Пример использования:

    <meta name="application-name" content="Имя приложения">

### Name `theme-color`

Указывает цвет вкладок для браузера

Пример использования:

    <meta name="theme-color" content="#000000" />

### Name `description`

Описание для документа. Ограничение до 150 символов.<br>
Используется для поисковых систем.

Пример использования:

    <meta name="description" content="Описание страницы">

### Name `robots`

Управление поведением поисковых машин при осмотре и индексации сайта.

Пример использования

    <meta name="robots" content="noindex">

В этом примере тег `meta` с атрибутом `robots` запрещает поисковым системам показывать страницу в результатах поиска.

### Name `google`

Пример использования

    <meta name="google" content="notranslate">\

### http-equiv `Content-Security-Policy`

Позволяет контролировать, откуда загружаются ресурсы.<br>
Применяется только к ресурсам, которые объявлены после него.

Пример использования

    <meta http-equiv="Content-Security-Policy" content="default-src 'self'">

## Протокол Open Graph

Протокол Open Graph - это микроразметка, позволяющая сделать ваш сайт наиболее привлекательным при его размещении в соцсетях. Изначально была создана компанией Facebook и работала только в ней.

### Property `og:title`

Заглавие страницы (чаще всего берут из тега title).

Пример использования

    <meta property="og:title" content="Заглавие страницы">

### Property `og:description`

Описание сайта.

Пример использования

    <meta property="og:image" content="assets/image.jpg">

### Property `og:url`

Ссылка на данную страницу. Если сайт много страничный, то данный тег указывается на каждой странице.

Пример использования

    <meta property="og:url" content="https://google.com">

### Property `og:locale`

Язык описания данной страницы.

Пример использования

    <meta property="og:locale" content="en_GB" />
