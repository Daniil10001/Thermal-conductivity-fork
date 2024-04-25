# Thermal-conductivity
## Как это запускать?
надо чё-то мудрое написать тут

## Как оно работает?
### Делаем сетку
Наша задач сводится к численному решению уравнения в частных произвдных. Для этого интересующая нас рассчётная область делится на сетку, в каждой ячейке которой мы будем считать температуру.
В работе использована структурированная прямоугольная рассчётная сетка, её размеры и шаг пользователь может менять в мейне (на предельных параметрах программа работает достаточно интересно).

### Как будем считать?

на умноформульном


### Задаём начальные условия
Чтобы начать рассчёт, на нужно от чего - то отталкиваться, поэтому необходимо задать начальные условия.

Граничные условия - это температура или закон, по которому она изменяется в граничных ячейках сетки, то есть в рамке, окаймляющей нашу рассчётную область.
Будем считать, что температура на границе не меняется и равна $
{T_{max}}$, а вот вещество внутри будет нагреваться от ${T_{0}}$.

Для каждого рассчёта солвер уникален:

Шаг по сетке мы вибираем сами , а вот шаг по времени рассчитывается автоматически. Так как мы решаем дифференциальное уравнение, то шаг по времени должен быть мал относительно шага по температуре.
Зная ${T_{max} - T_{min}}$ можно подобрать соответствующий ${dt}$, умножив приведённую разность на эмпирически (а может и нет, мы ещё не на третьем курсе) подобранный коэффициент ${\alpha}$  

### Наконец, считаем!!!

Запускаем рассчёт и наблюдаем за красотой (или не красотой, если поставили плохии начальные условия).

## Погодите, это реально?



