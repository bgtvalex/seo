# SEO

## HTML

### 1. Мета теги, описание, заголовок, контент, семантика

    1. <html lang="ru">
    2. <meta charset="utf-8" />
    3. <meta name="viewport" content="width=device-width, initial-scale=1" />
    4. <title>Excel To JSON Converter</title>
    	* закидываем больше ключевых слов
    	* на каждой странице ставим уникальный заголово
    5. <meta name="description" content="Легкий задачники для проектов" />
    	* больше ключевых слов
    	* уникальность
    6. Секции
    	* <header></header>
    	* <nav></nav>
    	* <main></main>
    	* <section></section>
    	* <article></article>
    	* <footer></footer>
    7. Заголовки
    	* <h1></h1>
    		* один на страницу
    		* важен так же как и title
    	* <h2></h2><h3></h3><h4></h4><h5></h5><h6></h6> - поддерживает иерархию
    8. Элементы
    * <button>Кнопка</button>
    	* <a href="#!" target="_blank">Ссылки</a>
    	* <p>текст в параграфы</p>
    	* для списков использовать:
    			* <ul>
    				* <li>item</li>
    				* <li>item</li>
    			* </ul>

## 2. Open graph

    * без OpenGraph
    	* https://ya.ru
    	* OpenGraph
    		* https://ya.ru
    		* заголовок
    		* описание
    			* изображение
    * Реализация
    	* <meta property="og:type" content="website" />
    	* <meta property="og:url" content="https://bgtvalex.ru" />
    	* <meta property="og:img" content="https://bgtvalex.ru/img/favicon.png" />
    	* <meta property="og:title" content="bgtvalex" />
    	* <meta property="og:description" content="wev-developer" />

## 3. Валидация HTML

    * [WC3](https://validator.w3.org/)

## 4. Canonical ссылки и человеко понятные урлы (ЧПУ)

    * Не читабельная ссылка
    	* http://cars.qq/auto/123/model/456
    * Читабельная ссылка - ЧПУ
    	* http://cars.qq/auto/bmv/model/m5
    * В ссылках тоже используются ключевые слова
    * Защищенный протокол
    	* httpS://cars.ru
    	* Canonical
    		* <link rel="https://bgtvalex.ru" href="https://bgtvalex.ru">
    		* две ссылки могут ссылаться на одну и ту же страницу, это дубликаты, плохо ранжируются
    			* для этого используют canonical ссылки в <head></head>

## 5. Индексация, meta robots, файл robots.txt

    * robots
    	* <meta name="robots" content="index"> - индексируется
    	* <meta name="robots" content="noindex"> - не индексируется
    	* <meta name="robots" content="follow"> - разрешает боту ходит по внутренним ссылкам
    	* <meta name="robots" content="nofollow"> - запрещает боту ходит по внутренним ссылкам
    	* <meta name="googlebot" content="noindex"> - запрещает Google индексировать страницу
    	* <meta name="yandexbot" content="index"> - разрешает Яндексу индексировать страницу
    * robots.txt
    		User-agent: yandex
    		disallow: /admin/*
    			sitemap: https://site.ru/sitemap.xml
    		User-agent: googlebot
    		disallow: /contacts
    		disallow: /admin/*
    			sitemap: https://site.ru/sitemap.xml

## 6. Sitemap

    * ссылка указывается в robots.txt
    * размер ограничен 500 КБ, иначе игнорируется
    * при превышении лимита sitemap разбивают на две и более частей

## 7. Краулинговый бюджет

    * кол-во страниц + частота обновления
    * битые, дублированные, админские ссылки

## 8. Web vitals. Метрики. Оптимизация. Доступность. FCP/LCP, FID, CLS.

    	* Core Web Vitals
    	* LCP - Largest Contentful Paint - скорость загрузки
    	* FID - First Input Delay - время когда пользователь может вводить первые данные
    	* CLS - Cumulative Layout Shift - при загрузке страницы, отображенный элемент не должен смещаться при загрузке следующего
    	* [PageSpeed Insights](https://pagespeed.web.dev/) - проверка
    	* lighthouse - локальная проверка в браузере
    	* tab / стрелочки / enter / escape / focus

## 9. Мобильные устройства. AMP

    	* AMP - фреймворк для веб компонентов, для мобильно версии сайта
    	* [amp](https://amp.dev/about/websites)

## 10. Редиректы, навигация

    * с www на без www
    	* с http на https
    	* со страниц без / на страницы со / в конце
    	* со страниц в верхнем регистре на нажний
    	* с index.php и /index.html на главную страницу

## 11. Микроразметка

    * [статья](https://habr.com/ru/companies/click/articles/486764/)
    * [Яндекс.Справка](https://yandex.ru/support/webmaster/schema-org/)
    * [Яндекс.Валидатор](https://webmaster.yandex.ru/tools/microtest/)
    * [schema.org](https://validator.schema.org/)

## 12. SSR и SPA

	* одними средствами SPA не возможно конкурировать с SSR
