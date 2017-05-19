[![Build Status](https://travis-ci.org/Sammers21/math_stat_python.svg?branch=master)](https://travis-ci.org/Sammers21/math_stat_python)

# Как делать задания?

Привидённые python-скрипты это пример, где вам нужно понять, что поменять так, что бы все работало для вашего варианта. По этой же причине код был написан и прокомментирован.

# Как запустить?

```
$ git clone https://github.com/Sammers21/math_stat_python
$ cd math_stat_python
$ python problem<номер_задачи>.py
```

**Заметка:** для запуска всех задач необходимы python-библиотеки: scipy, numpy, matplotlib, pandas, statsmodels. Версия python 3.5.2 или выше



# Вопросы к заданию номер 1

### №1

**Вопрос:** Как можно сгенерировать ваше распределение с использованием лишь равномерного распределения R(0,1)?

**Ответ:** Находим обратную функцию и подставляем значения равномерного распределения.

### №2

**Вопрос** (вытекающий из первого): А какая обратная функция к вашей?

**Ответ:** Взял мел и написал её на доске или бумаге.

### №3

**Вопрос:** Что такое медиана и какова медиана вашего распределения?

**Ответ:** Медиана — квантиль уровня 0.5, т.е. такое значение распределения, получить значение меньше которого можно с вероятностью 1/2. Чтобы найти его, нужно решить уравнение вида F(x) = 1/2, где F - функция распределения.

### №4

**Вопрос:** Дайте определение центральной предельной теоремы (ЦПТ)

**Ответ:**

![2017-03-09_20-37-36](https://cloud.githubusercontent.com/assets/8942211/23763400/8225d030-050a-11e7-87fc-80bf28ab529e.jpg)

### №5

**Вопрос:** Что такое дисперсия?

**Ответ:** Дисперсия: D(X) = E((X-E(X))^2)

# Вопросы к заданию номер 2

### №1

**Вопрос:** Что такое ошибка первого и второго рода?

**Ответ:**

![screenshot from 2017-03-05 21-20-44](https://cloud.githubusercontent.com/assets/16746106/23590054/1ec50b28-01ea-11e7-93da-3511d45e1e24.png)

### №2

**Вопрос:** Что такое уровень доверия?

**Ответ:** Уровень доверия — статистический термин, означающий вероятность того, что доверительный интервал содержит истинное значение параметра.

### №3

**Вопрос:** А какую вы будете использовать статистику для оценки:

			a) мат ожидания с известной дисперсией
			б) мат ожидания с неизвестной дисперсией
			в) дисперсии с известным мат ожиданем
			г) дисперсии с неизвестным мат ожиданем
	
**Ответы на a) и б)**

![image](https://cloud.githubusercontent.com/assets/16746106/23589495/42427c94-01df-11e7-8291-6169fdc557a0.png)

**Ответы на в) и г)**

![screenshot from 2017-03-05 20-03-24](https://cloud.githubusercontent.com/assets/16746106/23589484/0e09ba3c-01df-11e7-934a-f6787ce6a1ea.png)

# Вопросы к заданию номер 3

### №1

**Вопрос:** Приведите пример выборки, для которой коэффициент Пирсона будет близок к нулю, а Спирмена — к единице

**Ответ:** Выброс, см. пример на нижеприведенной иллюстрации

![pidr](http://i.imgur.com/mGFabdO.png)

### №2

**Вопрос:** При каких условиях коэффициент *такой-то* будет принимать крайнее значение *такое-то*

**Ответ:**

| к-т \ значение | -1 | 1 |
|----------------|----|---|
| Пирсона | `y = ax + b, a < 0` (обратная линейная связь) | `y = ax + b, a > 0` (прямая линейная связь) |
| Спирмена | `x_i > x_j => y_i < y_j` (строго обратная связь) | `x_i > x_j => y_i > y_j` (строго прямая связь) |

### Вклад

##### Каждый из вас, кто читает это README может помочь своим однокурсникам.

- Если тут нет вопроса, который Фурманов задавал вам, то не стесняйтесь и добавьте его (посредством pull request).
- Если у вас есть проблема, с которой вы столкнулись и не можете решить, то создайте issue в этом репозитории. Помощь обязательно будет. Быстрая и оперативная.
- Если вы считаете, что в коде, который демонстрирует примерное решение задачи, есть ошибка, то непременно исправьте её или сообщите о ней.
