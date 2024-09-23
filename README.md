# Аналитика продаж кофеен

Инструменты: Excel

## Исходные данные

Набор данных [Coffee Shop Sales](https://www.kaggle.com/datasets/ahmedabbas757/coffee-sales) размещен на kaggle.

Этот набор содержит информацию о транзакциях, совершенных в трех кофейнях одной сети. Присутствует информация о месте покупки, количестве товара и цене.

**Поля таблицы:**

- transaction_id: уникальный последовательный идентификатор, представляющий отдельную транзакцию;
- transaction_date: дата транзакции (ММ/ДД/ГГ);
- transaction_time: временная метка транзакции (ЧЧ:ММ:СС);
- transaction_qty: количество проданных товаров;
- store_id: уникальный идентификатор кофейни, где была совершена транзакция;
- store_location: местоположение кофейни, где была совершена транзакция;
- product_id: уникальный идентификатор проданного продукта;
- unit_price: розничная цена проданного продукта;
- product_category: описание категории продукта;
- product_type: описание типа продукта;
- product_detail: описание детали продукта.

Кроме того, было добавлено еще одно поле, в котором содержится стоимость всей покупки (количество x цена).

- purchase_price: сумма покупки.

<p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-1.JPG" alt="Рис 1" />
</p>

## Продажи по месяцам

На основании исходных данных была создана сводная таблица, отражающая прибыль сети кафеен по 6 месяцам. По полученной таблице можно сделать вывод, что прибыль немного упала к февралю, а потом стабильно росла к летним месяцам. Максимальная отметка в 166.486 $ достигнута в июне.

<p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-2.JPG" alt="Рис 2" />
</p>

Более наглядно распределение полученной прибыли отражено на графике.

<p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-3.JPG" alt="Рис 3" />
</p>

## Топ 5 типов и категорий продуктов

С помощью сводных таблиц были установлены самые часто покупаемые категории и типы продуктов. Среди категорий ожидаемо кофе занимает первое место, а за ним следует чай. По типам самым популярным является чай "Brewed Chai tea", а только второе и третье места занимают кофе "Gourmet brewed coffee" и "Barista Espresso".

<p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-6.JPG" alt="Рис 6" />
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-4.JPG" alt="Рис 4" />
</p>

Линейчатые диаграммы отражают количество самых популярных категорий и типов.

<p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-7.JPG" alt="Рис 7" />
</p>

 <p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-5.JPG" alt="Рис 5" />
</p>

## Распределение транзакций по часам

Группировка транзакций по часам в сводной таблице позволяет отследить наиболее прибыльные часы рабочего дня. По полученной таблице можно заметить, что наибольшее количество покупок совершено в промежутке с 8 до 10 часов, после чего количество продаж держется около медианы данных (около 9.000) в промежутке от 11 до 17 часов, а затем начинает падать и достигает минимума всего дня в 20 часов.

<p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-8.JPG" alt="Рис 8" />
</p>

Гистограмма, полученная по сводной таблице, демонстрирует описанное распределение данных.

<p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-9.JPG" alt="Рис 9" />
</p>

## Доли прибыли кофеен

Также можно определить прибыль каждой кофейни с помощью сводной таблицы. По её данным можно увидеть, что доход примерно одинаков.

<p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-10.JPG" alt="Рис 10" />
</p>

Доли вклада каждой кофейни демонстрируют круговые диаграммы. По ним также видно примерно одинаковое распределение процентов.

<p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-11.JPG" alt="Рис 11" />
</p>

## Дашборд

Все созданные графики объединены в один дашборд для более полного анализа продаж. Кроме графиков были размещены срезы, позволяющие осуществлять фильрацию по различным признакам.

Среди них срезы:

- Product category (категория продуктов)
- Month (доступные месяцы с января по июнь)
- Hour (рабочии часы кофейн с 6:00 до 20:00)
- Store location (одна из трех кофейн)

<p align="center">
    <img src="https://github.com/darazazulina/Coffee_shop_sales/blob/main/images/pic-12.JPG" alt="Рис 12" />
</p>

Дашборд позволяет по графикам наблюдать статистику, а такжеинтерактивно с ними взаимодействовать.
