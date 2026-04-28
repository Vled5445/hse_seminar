# hse_seminar


# Домашнее задание: Яндекс Cloud и PySpark

## Что сделано

Собрал витрину `mart_city_top_products` с топ-2 товарами по выручке для каждого города. Использовал PySpark в Zeppelin на Yandex Cloud.

## Данные

Три таблички: пользователи, заказы и товары. Всё создавал прямо в ноутбуке.

## Что происходит в коде

1. Считаю выручку: `revenue = qty * price`
2. Джойню заказы с пользователями и товарами
3. Группирую по городу и товару, считаю количество заказов, сумму qty и выручку
4. Через оконную функцию выбираю топ-2 товара по выручке в каждом городе
5. Сохраняю результат в S3 и локально в parquet
6. Читаю обратно и показываю

Скриншоты с настройкой y.cloud + запуском кода Spark

<img width="980" height="838" alt="Снимок экрана 2026-04-27 в 21 57 27" src="https://github.com/user-attachments/assets/26d935b6-5c24-49c3-a6a0-43c801fc9ea3" />

<img width="934" height="844" alt="Снимок экрана 2026-04-27 в 22 25 03" src="https://github.com/user-attachments/assets/27d4daed-dc7e-451a-a7c7-bdc4a1741cea" />

<img width="857" height="574" alt="Снимок экрана 2026-04-27 в 22 28 00" src="https://github.com/user-attachments/assets/aa4003bd-6393-4821-b1e0-121992066560" />


<img width="1433" height="356" alt="Снимок экрана 2026-04-27 в 22 47 01" src="https://github.com/user-attachments/assets/9205f507-4d44-46e1-9726-7b15a1fa9df7" />

<img width="1057" height="573" alt="Снимок экрана 2026-04-27 в 22 50 13" src="https://github.com/user-attachments/assets/7849db04-f2ef-4cb4-89e5-06f35bc754d3" />

<img width="687" height="481" alt="Снимок экрана 2026-04-27 в 22 56 33" src="https://github.com/user-attachments/assets/be2a7cc9-7192-4ad1-822b-2a36d59bbd30" />


<img width="894" height="503" alt="Снимок экрана 2026-04-27 в 22 57 20" src="https://github.com/user-attachments/assets/c0e459a1-c91b-427e-91c8-a225e3931e4d" />


<img width="729" height="480" alt="Снимок экрана 2026-04-27 в 22 57 33" src="https://github.com/user-attachments/assets/7c7be699-5d22-4771-8090-9926d7b7faf5" />
