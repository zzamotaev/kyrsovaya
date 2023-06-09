# База данных магазина корейской косметики

Этот репозиторий содержит базу данных, которая содержит информацию о продуктах и покупателях корейской косметики. База данных была разработана и создана командой специалистов по косметике и базам данных, с целью упростить и улучшить процессы управления продажами и отслеживания инвентаря.

## Структура базы данных

База данных состоит из двух основных таблиц: `products` и `customers` и нескольких похожих. 

### Таблица `products`

Таблица `products` содержит информацию о продуктах корейской косметики, включая их название, бренд, категорию, цену и количество на складе. Эта таблица была разработана с учетом нужд наших клиентов, чтобы обеспечить максимальную прозрачность и эффективность в управлении складом. Структура таблицы выглядит следующим образом:

| Поле             | Тип данных       | Описание                                    |
|------------------|-----------------|---------------------------------------------|
| id               | INT             | Уникальный идентификатор продукта            |
| product_name     | VARCHAR(255)    | Название продукта                           |
| brand            | VARCHAR(255)    | Бренд продукта                              |
| category         | VARCHAR(255)    | Категория продукта                          |
| price            | DECIMAL(10,2)   | Цена продукта                               |
| quantity_in_stock| INT             | Количество продукта на складе                |

### Таблица `customers`

Таблица `customers` содержит информацию о покупателях, включая их имя, адрес и номер телефона. Эта таблица была разработана с учетом нужд наших клиентов, чтобы обеспечить максимальную удобность в управлении заказами и лояльность наших покупателей. Структура таблицы выглядит следующим образом:

| Поле             | Тип данных       | Описание                                    |
|------------------|-----------------|---------------------------------------------|
| id               | INT             | Уникальный идентификатор покупателя          |
| customer_name    | VARCHAR(255)    | Имя покупателя                              |
| customer_address | VARCHAR(255)    | Адрес покупателя                            |
| customer_phone   | VARCHAR(20)     | Номер телефона покупателя                   |

## Импорт базы данных

Чтобы импортировать эту базу данных, вам нужно выполнить следующие шаги:

1. Скачайте файл `cosmetic_shop.sql`, который находится в корне репозитория.

2. Запустите свой клиент MySQL и подключитесь к базе данных.

3. Используйте команду `SOURCE` в командной строке MySQL, чтобы загрузить файл `cosmetic_shop.sql` в базу данных. Например: 

```
SOURCE /path/to/cosmetic_shop.sql;
```

## Лицензия

Эта база данных распространяется под лицензией [MIT](https://choosealicense.com/licenses/mit/), что означает, что вы можете свободно использовать, изменять и распространять эту базу данных в любых целях, при условии, что вы сохраните авторские права и дисклеймер в файле README. 

## Контакты

Если у вас есть какие-либо вопросы или замечания относительно этой базы данных, пожалуйста, свяжитесь с нами, используя информацию на странице контактов нашего сайта. Мы будем рады помочь вам!
