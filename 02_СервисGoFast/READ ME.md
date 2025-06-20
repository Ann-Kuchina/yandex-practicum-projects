# Исследование для сервиса аренды самокатов GoFast

## Цель проекта

Определить основной сегмент пользователей сервисом, определить факторы, влияющие на размер выручки,а также проверить следующие гипотезы:

1. Тратят ли пользователи с подпиской больше времени на поездки?
2. Среднее расстояние, которое проезжают пользователи с подпиской за одну поездку, не превышает 3130 метров? (оптимальным расстоянием считается 3130 метров с точки зрения износа самоката, данная гипотеза поможет нам предотвартить лишние потери)
3. Будет ли помесячная выручка от пользователей с подпиской по месяцам выше, чем выручка от пользователей без подписки - это необходимо для того, чтобы определить, на какую долю пользователей нам работать выгоднее.

## Общий вывод

Изучив данные в разрезе категорий подписок, мы можем сказать, что:
- пользователи с подпиской совершают поездки либо длительностью около 18-19 минут, либо на расстоянии около 3100-3200 метров;
- пользователи без подписки либо совершают поездки по времени около 17 минут, либо в среднем преодолевают расстояние около 3000-3100 метров
- коэффициент корреляции Пирсона в обоих случаях показывает, что данные о расстоянии и продолжительности поездки слабо коррелируют друг с другом. (0.49 и 0.55 соответственно)
Таким образом, пользователи с подпиской проезжают на 100м дальше или на 1 минуту дольше.

Мы также определили долю несовершеннолетних среди всех пользователей и нашу целевую аудиторию.
Доля несовершеннолетних составляет 5% от всех пользователей.
При этом основной возраст пользователей составляет от 20 до 30 лет.

1. Мы определили, что необходимо **отвергнуть нулевую гипотезу** в пользу альтернативной. То есть мы можем утверждать, что среднее время поездки пользователей обеих категорий одинаковое.
2. Мы определили, что **отвергнуть нулевую гипотезу нельзя**, то есть нельзя утверждать, что в среднем пользователи с подпиской проезжают больше 3130 метров за одну поездку.
3. Согласно результатам теста нам необходимо **отвергнуть нулевую гипотезу**, то есть мы не можем утверждать, что среднее значение помесячной выручки от подписчиков равно среднему значению выручки от пользователей без подписки.

## Используемые инструменты
Pandas, numpy, scipy.stats, matplotlib.pyplot, seaborn
