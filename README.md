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
### Проект 1: Анализ данных по обращениям граждан на Портал
 Задача №1
 - Выделите 10 самых частых тематик обращений.
 - Постройте диаграмму, иллюстрирующую топ-10 самых частых обращений за весь период.
 - Постройте диаграмму динамики по дням для топ-3 обращений.
 - Посчитайте суммарное время диалога (OperTime) для каждого проекта.

 Задача №2
 - Установите тикет в каждом из соответствующих ID обращений.
 - По какой из версий порталов эти тикеты были заведены.
 - В виде сводной таблицы укажите, сколько именно было тикетов по старой и новой версиям Портала.

 Задача №3
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
  <li>Итог №3.</li> Основное количество тикетов за проверяемый период было по старой версии Портала, почти 94%. Количество обращений с типом "Вопрос" через проект "GosUslugi_2LTP" равно 143. 
</ol>
<br> 

<br> 
### Проект 2: Анализ данных по обращениям граждан на Портал
 Задача №1
 - Выделите 10 самых частых тематик обращений.
 - Постройте диаграмму, иллюстрирующую топ-10 самых частых обращений за весь период.
 - Постройте диаграмму динамики по дням для топ-3 обращений.
 - Посчитайте суммарное время диалога (OperTime) для каждого проекта.

 Задача №2
 - Установите тикет в каждом из соответствующих ID обращений.
 - По какой из версий порталов эти тикеты были заведены.
 - В виде сводной таблицы укажите, сколько именно было тикетов по старой и новой версиям Портала.

 Задача №3
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

