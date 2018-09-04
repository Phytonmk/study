
# Обработка результатов наблюдения

Измерения делятся на:

* Прямые -- число со шкалы прибора считаем количетсвом физической величины
* Косвенны -- измерения, при котором расчётная физическая величина находится расчётным путём по известной зависимости (вроде тока через напряжение)
* Совместны -- косвенные, но с нахождением двух величин
* Совокупные -- одновременно производимые измерения нескольких одноименных величин, при котором искомое находится решение системы уравнений

## Погрешности

![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=x-x_0=\Delta%20x)

### Классификация погрешностей измерений


По выявляемости

* Выявленные
* Невыявленные
* Устранимые
* Неустранимые

Делятся на

* Грубые
* Систематические
* Случайные

А также бывают

* Промахи
* Ошибки

Полная погрешность включает в себя все погрешности, а именно:

* Случайные
* Систематические
* Оператора
* Прибора

По способу вычисления

* Абсолютные ![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=\Delta) (записывается в единицах измерения)
* Относительные ![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=\delta)

### Приорная погрешность

Погрешность прибора, которым мы измереям физ. величину ![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=\theta)

Каждый прибор имеет класс точности ![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=\gamma) 

Определение точности прибора 

* Если класс точности указан без кружка ![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=\theta=(\gamma*k)/100)
* Если класс точности указан в кружке ![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=\theta=(\gamma*x)/100)
* В аналоговых приборах погрешность -- половина цены наименьшего деления
* Если прибор цифровой -- разряд последней цифры (пример: в секундомере 15.28 с -- погрешность 0.01с)

Набор экспериментов называется **выборкой**

Наиболее точное значение -- среднее арифметическое выборки

### Распределением Гаусса

Распределением Гаусса  — распределение вероятностей, которое в одномерном случае задаётся функцией плотности вероятности, совпадающей с функцией Гаусса:

![math formula](https://wikimedia.org/api/rest_v1/media/math/render/svg/b77e66e0cfdc9859e63d68b5309bb794ad7cd1aa)

![график гаусовой кривой](https://studfiles.net/html/19259/957/html_zbSxAPq1b7.fybs/img-sepP0A.png)

### Дисперсия

Диспе́рсия случа́йной величины́ — мера разброса значений случайной величины относительно её математического ожидания

![math formula](https://profmeter.com.ua/upload/medialibrary/102/dispersia.gif)

Можно воспринимать как *Размытость кривой Гауса*

## Алгоритм обработки данных прямых измерений

1. Записать выборку полученных результатов наблюдений

![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=X_1,X_2%20,..,%20X_N)

2. Устранить устранимые системные погрешности
3. Разранжировать выбору (от маленького к большому)
4. Определить разных ![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=R=X_max-X_min) и объём выборки, например в задании ![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=N=5) (![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=R) - размах выборки)
5. Вычислить выборочное среднее
6. Вычислить СКО (дисперсию, формула выше) результатов наблюдений
7. Проверка на промах:

* По ско

![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=(((s))/(\S_x))>=V_p_N)

* по размаху

![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=((x-x_i)/R>=U_r_n))

Если всё окей, пишем **Промахов нет**

8. Рассчёт СКО среднего

![math formula](https://studfiles.net/html/2706/253/html_FQnyfScZ9w.VMR5/img-7omHOB.png)

9. Рассчёт случайной погрешности

* По **Стюденту**

- формула

* По размаху

- формула

10. Приборная погрешность (указания к рассчёту выше)

11. Вычисление полной погрешности

![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=\delta\overline{x}=\sqrt[2]{\delta%20x^2+\theta^2})

12. Определение полной погрешности и результатов эксперимента

* Полная погрешность округляется до одной значашей цифры, если первая значашая цифра > 1
Если первая значашая цифра -- 1 (или 2), то оставляется 2 значащие цифры
* Среднее значение округляется до разряда погрешности

13. Вычисление относительной погрещности

14. Запись результатов измерений

![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=X=\overline{x}\pm\Delta\overline{x})

![math formula](http://www.sciweavers.org/tex2img.php?bc=White&fc=Black&im=jpg&fs=12&ff=arev&eq=P=95%), N = 5


## Сперсекрет

При коруглении .5 округляется до ближайшего чётного числа

---

### Сайт кафедры физики

[www.physicsleti.ru](http://physicsleti.ru)

### Литература

учебное пособие **Методы обработки результатов физического эксперимента**

* В.В. Макаров
* Б.Е. Соботковский
* И.Л. Шейнман