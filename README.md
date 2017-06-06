[![Build Status](https://travis-ci.org/Sammers21/math_stat_python.svg?branch=master)](https://travis-ci.org/Sammers21/math_stat_python)

# Как делать задания?

Приведённые python-скрипты это пример, где вам нужно понять, что поменять так, что бы все работало для вашего варианта. По этой же причине код был написан и прокомментирован.

# Как запустить?

```
$ git clone https://github.com/Sammers21/math_stat_python
$ cd math_stat_python
$ python problem<номер_задачи>.py
```

**Заметка:** для запуска всех задач необходимы python-библиотеки: scipy, numpy, matplotlib, pandas, statsmodels. Версия python 3.5.2 или выше

# Пример пояснительной записки к: 
    
**Номеру 4:**
    https://www.evernote.com/shard/s267/sh/20c765ce-65bd-4590-9455-72512dc2ad3a/1795f8e28d6b3966d58e94c024d9378b
    
**Номеру 5:**
https://www.evernote.com/shard/s267/sh/49f91974-1090-4d64-9315-60c0a1b80fc2/9bfe1f4704883bf9a8e0ba073188827e

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

# Вопросы к заданию номер 4

### №1

**Вопрос:** Классическая линейная нормальная регресионная модель.  
**Ответ:**  Если регрессионная модель отвечает данным условиям:  

* ![regression](https://latex.codecogs.com/gif.latex?Y_i%3D%5Cbeta_1&plus;%5Cbeta_2%5Ccdot%20X_%7B2%2Ci%7D&plus;...&plus;%5Cbeta_k%5Ccdot%20X_%7Bk%2Ci%7D&plus;%5Cvarepsilon_i)
* ![regressors](https://latex.codecogs.com/gif.latex?X_%7B2%2Ci%7D%2C%20...%2C%20X_%7Bk%2Ci%7D) — детерминированные (неслучайные) величины
* ![error_resriction](https://latex.codecogs.com/gif.latex?E%28%5Cvarepsilon_i%29%3D0%5Cqquad%20D%28%5Cvarepsilon_i%29%3D%5Csigma%5E2) (дисперсия ошибки постоянна - гомоскедастичность)
* ![noncorrelation](https://latex.codecogs.com/gif.latex?E%28%5Cvarepsilon_i%5Ccdot%20%5Cvarepsilon_j%29%3D0%2C%20i%20%5Cneq%20j) — некоррелированность ошибок
* ![norm_distribution](https://latex.codecogs.com/gif.latex?%5Cvarepsilon_i%20%5Csim%20N%280%2C%5Csigma%5E2%29)

То она называется классической линейной нормальной регрессионной моделью (КЛНРМ)

### №2

**Вопрос:** Метод наименьших квадратов и теорема Гаусса-Маркова.  
**Ответ:**  МНК заключается в нахождении таких коэффициентов регрессии, при которых суммма квадратов ошибок будет наименьшей:  
![ols](https://latex.codecogs.com/gif.latex?%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20%28Y_i%20-%20%28%5Chat%7B%5Cbeta_1%7D&plus;%5Chat%7B%5Cbeta_2%7D%5Ccdot%20X_%7B2%2Ci%7D%20&plus;%20...%20&plus;%20%5Chat%7B%5Cbeta_k%7D%5Ccdot%20X_%7Bk%2Ci%7D%29%29%5E2%20%5Crightarrow%200)  
Берётся частная производная по каждому коэффиценту, приравнивается к нулю. Из таких уравнений составляется и решается система.  

Теорема Гаусса Маркова: если регрессионная модель удовлетворяет условиям Гаусса-Маркова (из вопроса 1), то:

* Полученные оценки коэффициентов несмещённые
* Оценки состоятельны
* Оценки эффективны, т.е. имеют наименьшую дисперсию среди всех возможных линейных оценок
* Оценки распределены нормально

### №3

**Вопрос:** Оценка дисперсии случайной составляющей и ковариационной матрицы оценок коэффициентов регрессии.  
**Ответ:**  
![error_varience](https://latex.codecogs.com/gif.latex?%5Chat%7B%5Csigma%7D%5E2%28%5Cvarepsilon%20%29%3D%5Cfrac%7BRSS%7D%7Bn-k%7D)  
*k* — количество оцениваемых коэффициентов  
![coef_covarience](https://latex.codecogs.com/gif.latex?%5Chat%7BV%7D%28%5Cbeta%29%3D%5Chat%7B%5Csigma%7D%5E2%28%5Cvarepsilon%29%5Ccdot%20%28X%5ET%5Ccdot%20X%29%5E%7B-1%7D)  

### №4

**Вопрос:** Коэффициент детерминации.  
**Ответ:** ![determination](https://latex.codecogs.com/gif.latex?R%5E2%3D%5Cfrac%7BESS%7D%7BTSS%7D%3D1-%5Cfrac%7BRSS%7D%7BTSS%7D)  
Это доля дисперсии зависимой переменной, объяснённая моделью. Принимает значения от 0 до 1. Чем он выше, тем лучше подобрана модель и больше зависимость объясняемой переменной от объясняющих.

### №5

**Вопрос:** Доверительный интервал для коэффициента регрессии.  
**Ответ:** ![interval](https://latex.codecogs.com/gif.latex?%5Cbeta_j%5E0%20-%20t_%7B1-%5Calpha/2%7D%5Ccdot%20%5Csqrt%7B%5Chat%7B%5Csigma%7D%5E2%28%5Cbeta_j%29%7D%20%5Cleq%20%5Chat%7B%5Cbeta_j%7D%20%5Cleq%20%5Cbeta_j%5E0%20&plus;%20t_%7B1-%5Calpha/2%7D%5Ccdot%20%5Csqrt%7B%5Chat%7B%5Csigma%7D%5E2%28%5Cbeta_j%29%7D)  
*t* — квантиль распределения *t(n-k)*

### №6

**Вопрос:** Проверка гипотезы о значении коэффициента и значимости регрессии в целом.  
**Ответ:** Из методички от [Zakhse](https://github.com/Zakhse):  
![](https://i.imgur.com/DaVRr68.png)  
![](https://imgur.com/OUj2RuZ.png)

### №7

**Вопрос:** Проверка гипотезы о линейном ограничении.  
**Ответ:** Из методички от [Zakhse](https://github.com/Zakhse):
![](https://imgur.com/7iLNZzO.png)  

# Вопросы к заданию номер 5

### №1

**Вопрос:** Интерпретация коэффициентов линейной, полулогарифмической и логарифмической моделей регрессии.  
**Ответ:** Из [статьи](https://github.com/bdemeshev/epsilon/raw/master/e_001/functional-form/functional-form.pdf) Фурманова К.К.:  
![](http://imgur.com/v99RhEB.png)

### №2

**Вопрос:** Тесты на правильность спецификации: график «остатки-прогнозы», тест Рамсея.  
**Ответ:** Читаем [статью](https://github.com/bdemeshev/epsilon/raw/master/e_001/functional-form/functional-form.pdf) Фурманова К.К.!  

# Вопросы к заданию номер 6

### №1

**Вопрос:** Линейная модель вероятности. Модели logit и probit, их оценивание методом
максимального правдоподобия.
 
**Ответ:**
 
![image](https://cloud.githubusercontent.com/assets/16746106/26805801/6cbfc3c2-4a56-11e7-95df-89a732d56349.png)
![image](https://cloud.githubusercontent.com/assets/16746106/26805842/a0116bc2-4a56-11e7-821d-3689cb2236fc.png)
![image](https://cloud.githubusercontent.com/assets/16746106/26805858/b8b0c9ca-4a56-11e7-9c99-7d3f6f84b0e3.png)

### №2

**Вопрос:** Интерпретация коэффициентов линейной и логит моделей.
 
**Ответ:**
- Для Logit:

![image](https://cloud.githubusercontent.com/assets/16746106/26806002/6aab445c-4a57-11e7-8861-bc102fa3f21e.png)
- Для линейной:

![image](https://cloud.githubusercontent.com/assets/16746106/26806051/9a7031e8-4a57-11e7-994d-116dd01a97ad.png)

### №3

**Вопрос:** Что такое Pseudo R^2?
 
**Ответ:** 

![image](https://cloud.githubusercontent.com/assets/16746106/26806141/0ea144b2-4a58-11e7-8773-16013afcea7b.png)

### Вклад

##### Каждый из вас, кто читает это README может помочь своим однокурсникам.

- Если тут нет вопроса, который Фурманов задавал вам, то не стесняйтесь и добавьте его (посредством pull request).
- Если у вас есть проблема, с которой вы столкнулись и не можете решить, то создайте issue в этом репозитории. Помощь обязательно будет. Быстрая и оперативная.
- Если вы считаете, что в коде, который демонстрирует примерное решение задачи, есть ошибка, то непременно исправьте её или сообщите о ней.