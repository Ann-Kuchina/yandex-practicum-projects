# Исследование объявлений о продаже квартир

## Цель проекта

В нашем распоряжении данные сервиса недвижимости --- архив объявлений о
продаже квартир в Санкт-Петербурге и соседних населённых пунктах за
несколько лет.

По каждой квартире на продажу доступны два вида данных. Первые вписаны
пользователем, вторые --- получены автоматически на основе
картографических данных.

Мы хотим изучить предоставленные данные и выявить закономерности
стоимости квартир в зависимости от различных факторов, а также провести
исследовательский анализ в отношении качества данных

## Общий вывод

1. В процессе работы были выявлены проблемы с данными, которые
заполняются клиентами: много пропусков, выбивающиеся нереалистичные
значения.
2. Норма продажи квартиры по времени - 3 месяца.
3. Факторы, влияющие на стоимость квартиры - общая площадь (логично), жилая площадь.
Остальная площадь квартиры оказывает незначительное влияние на
стоимость.

## Используемые инструменты

Pandas, numpy, matplotlib.pyplot, seaborn
