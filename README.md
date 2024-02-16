# Портфолио: аналитик данных

## :woman_technologist: Обо мне 
<div align="center">
<img src="https://media.giphy.com/media/W2KZgZo97jtC313Hn9/giphy.gif" width="500" height="300"/>
</div>

**Привет!** <br>
Меня зовут Светлана, я начинающий аналитик данных <img src="https://media.giphy.com/media/WUlplcMpOCEmTGBtBW/giphy.gif" width="30">  из г. Калининграда. <br>
- :telescope: Я окончила обучение по профессии аналитик данных. 

- :seedling: Интересуюсь и изучаю технические инструменты сбора, анализа и интерпретации информации для выявления закономерности и причинно-следственных связей в данных.

- :zap:  Надеюсь в составе специалистов команды вносить свой вклад в решение задач по улучшению бизнес-процессов.
<br>

В этом репозитории вы можете найти некоторые из моих проектов, выполненных во время обучения и практики.
<br>

## :hammer_and_wrench: Навыки и технологии
- Инструменты анализа данных: ``SQL``, ``Excel``: 
- Языки программирования и библиотеки: ``Python``, ``Pandas``, ``math`` 
- Системы управления базами данных: ``MySQL``, ``PostgreSQL``
- Средства визуализации данных: ``PowerBi``, ``Matplotlib``, ``seaborn``




## :clipboard: Проекты
### Проект 1. Анализ данных по обращениям граждан на Портал
 Задача №1:
 - Выделите 10 самых частых тематик обращений.
 - Постройте диаграмму, иллюстрирующую топ-10 самых частых обращений за весь период.
 - Постройте диаграмму динамики по дням для топ-3 обращений.
 - Посчитайте суммарное время диалога (OperTime) для каждого проекта.

 Задача №2:
 - Установите тикет в каждом из соответствующих ID обращений.
 - По какой из версий порталов эти тикеты были заведены.
 - В виде сводной таблицы укажите, сколько именно было тикетов по старой и новой версиям Портала.

 Задача №3:
 - Добавьте еще одну колонку, назовите ее «Флаг». Значение в этой колонке должно быть равно 1 в том случае, если значение в поле «Проект» равно GosUslugi_2LTP, а тип обращения — «Вопрос». В остальных случаях значение должно быть равно нулю. Посчитайте количество единиц в колонке «Флаг».

> #### Краткое описание решения
> Задача №1
> 
> 10 самых частых тематик обращений определили с помощью сводной таблицы, расположив в строки - столбец "Тиматика", в значения - "id" (по количеству). Использовали фильтр по значению при определении 10 первых тематик. Для визуализации выбрали наиболее подходящую, линейчатую диаграмму. Диаграмму динамики по дням построили посредством сводной таблицы, расположив в строки - "Дату", в столбцы - "Тематику", в значения - "id" (по количеству). Использовали фильтр для определения 3-топ. Для визуализации выбрали график, наиболее подходящий при отображении динамики по дням. Суммарное время диалога (OperTime) для каждого проекта рассчитали расположив в строках сводной таблицы - "название Проекта", в значении - сумму по полю "OperTime", перевели секунды в часы. 
>
> Задача №2
> 
> Тикет каждому из ID обращений и версии портала к нему присоединили с помощью функции ВПР из исходных данных по ID-ключу. Количество тикетов по старой и новой версиям рассчитали с помощью сводной таблицы, расположив в строки - столбец "Портал", в значения - количество по полю "Тикет".
> 
> Задача №3
> 
> Колонку «Флаг» со значением 1 в случае, когда значение в поле «Проект» равно GosUslugi_2LTP, а тип обращения — «Вопрос» создали применив функцию "ЕСЛИ" и "И". Количество посчитали функцией "СУММ". 

 <a href="https://github.com/SvetaPK/my_portfolio/blob/main/Excel_%D0%A2%D0%B5%D1%81%D1%82%D0%BE%D0%B2%D0%BE%D0%B5_1.xlsx">Ссылка на проект</a>
  (можно быстро посмотреть результаты работы)

#### <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1.</li> Из 10 наиболее частых тематик обращения граждан на Портал самой частой является тема "Получение услуги ведомства", её доля от всех обращений составляет 38% по 10 самым частым. Менее всего вопросов поступает по теме "Платежи(ИПШ)" и "Вопрос по ФЭР" - 1,4% у каждой.    
  <li>Итог №2.</li> Исходя из 3 самых массовых тематик обращений всплеск обращений наблюдается в начале с 2 декабря по 4 декабря и период с 8 декабря по 11 декабря. Возможно это связано с желанием граждан не оставлять не завершенные дела на следующий год. Чаще всего граждане предпочитают использовать Проект GosUslugi_ZagrPass, доля суммарного времени его использования от всех составляет 55,7%.   
  <li>Итог №3.</li> Основное количество тикетов за проверяемый период было по старой версии Портала, почти 94%. Количество обращений с типом "Вопрос" через проект "GosUslugi_2LTP" незначительное - 143, что составляет 1% от всех обращений. 
</ol>
<br> 

### Проект 2. Анализ интенсивности работы торговых точек
 Задача №1:
 - Постройте по дням динамику количества оплат по торговым точкам.

 Задача №2:
 - Для каждой торговой точки рассчитайте долю покупок, в которых цена превысила заданное значение.

 Задача №3:
 - Для каждого месяца покупки рассчитайте долю каждой торговой точки в общем объеме покупок (в рублях).

 Задача №4:
 - Постройте калькулятор. Параметрами (полями, которые может вводить/менять пользователь) должны быть торговая точка и дата. Калькулятор должен вывести сумму оплат, количество оплат и среднюю оплату по данной торговой точке за весь период вплоть до указанной даты.
   
 Задача №5:
 - Постройте прогноз объема оплат на следующий месяц. 


> #### Краткое описание решения
> Задача №1
> 
> Динамику количества оплат по дням по торговым точкам построили с помощью сводной таблицы, расположив в строки - столбец "date_payment", в столбцы - "address_shop", в значения - "id_purchase" (по количеству). Для визуализации выбрали график, наиболее подходящий при отображении динамики по дням. 
>
> Задача №2
> 
> Для наглядного отображения доли покупок по цене, превышающей заданное значение собрали калькулятор. С помощью функции "СЧЁТЕСЛИМН" рассчитали количество покупок по заданному условию. Создали столбцы со значениями доли покупок по каждой торговой точке. Построили диаграмму для визуализации соотношения Доли покупок по цене выше заданного значения и Доли покупок по цене до заданного значения.
> 
> Задача №3
> 
> Долю каждой торговой точки в общем объеме покупок (в рублях) для каждого месяца рассчитали с помощью сводной таблицы. Для визуализации использовали график.
>
> Задача №4
> 
> Для построения калькулятора с параметрами: торговая точка и дата, который выводит: сумму оплат, количество оплат и среднюю оплату по данной торговой точке за весь период вплоть до указанной даты использовали функции: "СУММЕСЛИМН", "СЧЁТЕСЛИМН" и "СРЗНАЧЕСЛИМН", при написании функции обращались к таблице с исходными данными.
> 
> Задача №5
> 
> Прогноз объема оплат на следующий месяц построили используя график, линию тренда. Во втором случае прогноз объема оплат на следующий месяц построили с помощью создания "Листа прогноза".
> 

<a href="https://github.com/SvetaPK/my_portfolio/blob/main/Excel_%D0%A2%D0%B5%D1%81%D1%82%D0%BE%D0%B2%D0%BE%D0%B5_2_%D0%A2%D0%BE%D1%80%D0%B3%D0%BE%D0%B2%D1%8B%D0%B5_%D1%82%D0%BE%D1%87%D0%BA%D0%B8.xlsx">Ссылка на проект</a>
  (можно быстро посмотреть результаты работы)

#### <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1.</li> Из 4 проверяемых торговых точек наибольшая интенсивность продаж у торговой точки по адресу ул. Ленина, 13/2, её доля составляет 42,7% от всего объёма.  Наименьший объем продаж у торговой точки по адресу Проспект Вернадского, 89. Распределение объема продаж по датам в течение мясяца в целом равномерное. 
  <li>Итог №2.</li> Создали калькулятор для наглядного отображения доли покупок по заданной цене. По всем торговым точкам доля покупок по цене выше 3000 руб. меньше, чем доля покупок по цене не превышающей 3000 руб.
  <li>Итог №3.</li> По месяцам наибольшая доля продаж в общем объеме продаж у торговой точки по адресу ул. Ленина, 13/2 (от 40% до 45%), наименьшая - у торговой точки по адресу Проспект Вернадского, 89 (от 11% до 17%). 
  <li>Итог №4.</li> Создали калькулятор который выводит: сумму оплат, количество оплат и среднюю оплату по данной торговой точке за весь период вплоть до указанной даты.
  <li>Итог №5.</li> Прогноз объема оплат на следующий месяц показал тенденцию к снижению общего объёма продаж. 
</ol>
<br>

### Проект 3. Калькулятор юнит-экономики онлайн-школы
 Задача №1. Собрать калькулятор юнит-экономики для того, чтобы понять, как должны измениться экономические показатели, чтобы добиться поставленных целей на следующий год:
 - Выйти на 4000 активных студентов.
 - Удержать маржинальность на уровне выше 15%.
 - Выйти на выручку выше 35 000 000 руб. в месяц.
 
 Задача №2. Добавить в калькулятор поправочный коэффициент и с его помощью пересчитать количество студентов на период с 05.21 по 04.22 для того, чтобы определить сколько новых пользователей нужно привести на платформу, чтобы выполнить план по новым платящим студентам.
 
 Задача №3. Пересчитать план найма преподавателей с учетом новых данных, изменив значения пропускной способности и ретеншена преподавателей.

> #### Краткое описание решения
> Задача №1
> 
> На листе "Свод" по историческим данным за период с 01.01.2020 по 30.04.2021 с помощью сводных таблиц собрали данные по: количеству уроков, количеству студентов, количеству новых студентов, среднюю цену одного урока. Рассчитали доли статей юнит-экономики и маржинальность на последний известный период - 04.2021. Для этого рассчитали показатели:
>  - Средний Retention (доля пользователей, которые использовали наш продукт в прошлом месяце и продолжили пользоваться им в текущем месяце),
>  - Lifetime (продолжительность обучения в месяцах),
>  - Средняя интенсивность (),
>  - Lifetime (уроки),
>  - Средняя цена урока,
>  - LTR (выручка от клиента за все время, показывает, сколько всего денег в среднем нам принесет один клиент за всё время использования наших услуг),
>  - САС (затраты на маркетинг и продажи  для конвертации потенциального клиента в  покупателя),
>  - ЗП Учителя на 1 урок,
>  - Fixed costs на 1 урок (постоянные затраты, которые не меняются с изменением объема производства).
>    
> На лист "Главный" собрали всю информацию, и историческую и рассчитанную, по месяцам. Для получения плана на следующий год продлили таблицу на 12 месяцев. Определили набор параметров (столбец "Показатели"), чтобы получить прогноз по всем значениям. Рассчитали их базовые значения на исторических данных (столбец "Факт 05.20-04.21") учитывая, что первые четыре месяца работы были установочные, для расчета используем период с 05.2020 по 04.2021. Добавили столбец "Изменение" для возможности вносить изменения показателей в процентном выражении на плановый период (столбец "05.21-04.22). Для получения новых значений показателей (с учетом изменений) используем формулу изменения показателя на указанный процент. 
> 
> Задача №2
> 
> Тикет каждому из ID обращений и версии портала к нему присоединили с помощью функции ВПР из исходных данных по ID-ключу. Количество тикетов по старой и новой версиям рассчитали с помощью сводной таблицы, расположив в строки - столбец "Портал", в значения - количество по полю "Тикет".
> 
> Задача №3
> 
> Колонку «Флаг» со значением 1 в случае, когда значение в поле «Проект» равно GosUslugi_2LTP, а тип обращения — «Вопрос» создали применив функцию "ЕСЛИ" и "И". Количество посчитали функцией "СУММ". 

 <a href="https://github.com/SvetaPK/my_portfolio/blob/main/Excel_%D0%A2%D0%B5%D1%81%D1%82%D0%BE%D0%B2%D0%BE%D0%B5_1.xlsx">Ссылка на проект</a>
  (можно быстро посмотреть результаты работы)






<p> Проект 2: Калькулятор юнит-экономики онлайн-кинотеатра</p>
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1</li>
  <li>Задача №2.</li>
</ol>

<p>Как решала(-а): краткое описание решения (автореферат)<p>

> <a href="https://drive.google.com/drive/folders/11HcEeqniyrCMjuwHZ0GLysX0A2SEv-_x">Ссылка на проект</a>
 (ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)
 
<p>Выводы (итоги):<p>
<ol>
  <li>Итог №1</li>
  <li>Итог №2</li>
</ol>
<br> 

<br> 
<p> Проект 3: Когортный анализ онлайн-кинотеатра с помощью SQL</p>
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1</li>
  <li>Задача №2.</li>
</ol>

<p>Как решала(-а): краткое описание решения (автореферат)<p>
  
> <a href="https://drive.google.com/drive/folders/1wdD-mfSeIsHWgrMLJz8Tv_ClAuP_EAOQ?usp=sharing">Ссылка на проект</a>
(ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)

  <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1</li>
  <li>Итог №2</li>
</ol>

<br> 
<p>Проект 4: Построение витрины для модели машинного обучения в банке </p> 
<p>Что нужно было сделать: задача №1.<p>
  
<p>Как решала(-а): краткое описание решения (автореферат)<p>

> <a href="https://drive.google.com/drive/folders/1QOk5AAh6x7jK_yHgfKI2sUFYR7AWUi5u">Ссылка на проект</a>
(ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)
  
 <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1</li>
  <li>Итог №2</li>
</ol>
<br> 


<p>Проект 5: Моделирование изменения балансов студентов</p> 
<p>Что нужно было сделать:<p>
<ol>
  <li>Задача №1</li>
  <li>Задача №2.</li>
</ol>

<p>Как решала(-а): краткое описание решения (автореферат)<p>

> <a href="https://github.com/Skyproportfolio/data-analytics-5month/blob/main/Проект%205.xlsx">Ссылка на проект</a>
(ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)
 
 <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1</li>
  <li>Итог №2</li>
</ol>

## :mailbox: Контактная информация
- Email: svetland35@gmail.com

