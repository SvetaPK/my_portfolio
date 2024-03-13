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
 
 Задача №2. Планирование найма преподавателей.
  
> #### Краткое описание решения
> Задача №1.
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
> На лист "Главный" собрали всю информацию, и историческую и рассчитанную, по месяцам. Для получения плана на следующий год продлили таблицу на 12 месяцев. Определили набор параметров (столбец "Показатели"), чтобы получить прогноз по всем значениям. Рассчитали их базовые значения на исторических данных (столбец "Факт 05.20-04.21") учитывая, что первые четыре месяца работы были установочные, для расчета используем период с 05.2020 по 04.2021. Добавили столбец "Изменение" для возможности вносить изменения показателей в процентном выражении на плановый период (столбец "05.21-04.22). Для получения новых значений показателей (с учетом изменений) используем формулу изменения показателя на указанный процент. Настроили условное форматирование. И построили калькулятор заполнив по месяцам данные, для этого:
> - значения "Retention" и "Интенсивность" притянули из соответствующих месяцев исторических данных и учли поправку из колонки "Изменение",
> - "план по ФОТ" и "план по новым студентам" нам дан, скопируем его в таблицу,
> - "Количество старых студентов" в 05.2021 рассчитаем с помощью "Количества студентов всего" за предыдущий месяц (04.2021)  и "Retention" за 05.2021, сложением определим "Количества студентов всего" за май. Распространим формулы на все месяца.
> - Количество "Регистраций" определим как отношение "Количество новых студентов" к "Конверсии в покупку",
> - Количество "Уроков" это произведение "Количества студентов всего" на "Интенсивность",
> - "Зарплата учителей" это произведение "Количества уроков" на "Оплату учителя за 1 урок",
> - "Выручка" это произведение "Количества уроков" на "Фактическую цену за 1 урок",
> - "Расходы на маркетинг" это произведение количества "Регистраций" на прогнозный "СРА",
> -  Рассчитали доли статей юнит-экономики по месяцам и маржинальность для прогнозного периода.
>
> Для визуализации юнит-экономики использовали круговую диаграмму для фактических показателей и плановых показателей.
> Создали график - комбинированную диаграмму с "Выручкой" и "Количеством студентов" по месяцам.
> Внесли рекомендуемые изменения показателей. Все плановые значения изменились автоматически Результаты отразились на графиках.
> Создали визуализацию плановых расходов на маркетинг и регистрации новых пользователей. Лист "План Маркетинга". 
> 
> Задача №2
> 
> На листе "Найм П" для планирования найма преподавателей рассчитаем время самого первого урока преподавателя, чтобы определить количество новых преподавателей в каждом месяце. Для подсчета уникальных преподавателей используем "Модель данных". Рассчитали по месяцам количество преподавателей "новых", "старых" и "всего", Retention, количество уроков, Интенсивность, Пропускная способность П. Для калькулятора набор параметров будет следующим: Средний Retention, средняя пропускная способность преподавателя. Сопоставим количество уроков, которое мы сможем провести с количеством уроков, которое нам придется провести. Для визуализации используем график. График показал, что необходимо скорректировать план найма. Введем столбец "Ошибки модели", который будет равен разности Пропускной способности и количества уроков, чтобы исключить отрицательные числа введем квадрат разности. Рассчитаем сумму квадратов ошибок. Для корректировки плана найма используем инструмент Excel, который подгонит значения максимально точно - Поиск решения, его задача минимизировать сумму квадратов ошибок меняя значения найма преподавателей. Установим ограничение на значении 60 и получим скорректированный план найма учителей.
> 

<a href="https://github.com/SvetaPK/my_portfolio/blob/main/Excel_%D0%A2%D0%B5%D1%81%D1%82%D0%BE%D0%B2%D0%BE%D0%B5_3_%D0%A1%D0%B1%D0%BE%D1%80%D0%BA%D0%B0_%D0%BA%D0%B0%D0%BB%D1%8C%D0%BA%D1%83%D0%BB%D1%8F%D1%82%D0%BE%D1%80%D0%B0_%D1%8E%D0%BD%D0%B8%D1%82_%D1%8D%D0%BA%D0%BE%D0%BD%D0%BE%D0%BC%D0%B8%D0%BA%D0%B8.xlsx">Ссылка на проект</a>
  (можно быстро посмотреть результаты работы)

#### <p>Выводы (итоги):<p>
<ol>
  <li>Итог №1.</li> Использование калькулятора юнит-экономики позволило решить вопрос: как следует изменить (увеличить/уменьшить) значения экономических показателей, чтобы добиться поставленных целей в следующем году. Для этого потребуется: снизить Средний СРА на 10%, увеличить Конверсию в покупку на 10,5%, увеличить Retention на 3%, увеличить Интенсивность на 13%, уменьшить Долю скидок на 30%, можно увеличить зарплату учителей на 15%. В результате получим маржинальность более 18%, число активных студентов станет более 4000, выручка за месяц составит 33904340 рублей.      
  <li>Итог №2.</li> График сопоставления необходимого количества уроков с количеством уроков, которое способны провести преподаватели показал, что летом количество уроков, которое надо будет провести будет невысоким, но уже в сентябре возможен дефицит преподавательских ресурсов, который будет дальше усугубляться. Применение инструмента Excel - Поиск решения, позволило скорректировать план найма учителей.
</ol>
<br> 

### Проект 4. Когортный анализ
Проанализируйте клиентский LTV по когортам и сделайте выводы:						
какие когорты лучше, а какие хуже с точки зрения LTV.	

 Задача №1:
Постройте сводную таблицу с абсолютным ретеншеном клиентов по месячным когортам.				

 Задача №2:
Постройте таблицу с относительным базовым ретеншеном.			

 Задача №3:
На основании ретеншена рассчитайте лайфтайм с помощью метода усредненных прямоугольников для каждой когорты.		

 Задача №4:
Рассчитайте LTR для каждой когорты с помощью ARPU. Предположите, что ARPU = 300.

 Задача №5:
Рассчитайте LTV с помощью усредненных костов для каждой когорты.			

 Задача №6:
Сделайте выводы относительно хороших и плохих когорт с точки зрения LTV.						
Для этого выделите:						
 - когорту, которая показывает высокий LTV за счет высокого лайфтайма;						
 - когорту, которая показывает высокий LTV за счет низких костов;						
 - когорту, которая показывает низкий LTV за счет низкого лайфтайма;						
 - когорту, которая показывает низкий LTV за счет высоких костов.
  							
 Задача №7:
Посчитайте суммарную прибыль нашей компании по всем клиентам (за всё время).							
На сколько процентов изменится суммарная прибыль, если увеличить ARPU на 10%?	

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


## :mailbox: Контактная информация
- Email: svetland35@gmail.com

