# Исследование причин убытков развлекательного приложения Procrastinate Pro+

**Описание данных:**  
Каждая запись в логе — это действие пользователя, или событие.   
Датафрейм visits:   
* user_id — уникальный идентификатор пользователя;  
* region — страна пользователя;  
* device — тип устройства пользователя;  
* channel — идентификатор источника перехода;  
* session_start — дата и время начала сессии;  
* session_end — дата и время окончания сессии.

Датафрейм orders:   
* user_id — уникальный идентификатор пользователя;  
* event_dt — дата и время покупки;  
* revenue — сумма заказа.  

Датафрейм costs:   
* dt — дата проведения рекламной кампании;  
* channel — идентификатор рекламного источника;  
* costs — расходы на эту кампанию.  

**Цель исследования:**
найти причины убытков развлекательного приложения Procrastinate Pro+.

**Задачи исследования:**  
1. Привести в необходимый вид данные для проведения анализа.  
2. Задать функции для расчёта и анализа LTV, ROI, удержания и конверсии. 
3. Провести исследовательский анализ данных.
4. Проанализировать расходы на маркетинг. 
5. Оценить окупаемость рекламы. 
6. Выделить причины неэффективности привлечения пользователей.
7. Сформулировать рекомендации для отдела маркетинга.

**Ход исследования:**  
Данные для проведения исследования я возьму из файлов — visits_info_short.csv ('/datasets/visits_info_short.csv'), orders_info_short.csv ('/datasets/orders_info_short.csv'), costs_info_short.csv ('/datasets/costs_info_short.csv').  
В начале исследования данные из файла я проверю на пропуски, аномалии, ошибки, дубликаты. Затем задам функции, необходимые для проведения исследования: функции для вычисления значений метрик и функции для построения графиков.  
Для проведения исследовательского анализа данных составлю профили пользователей, выясню из каких стран пользователи приходят в приложение и на какую страну приходится больше всего платящих пользователей, узнаю какими устройствами пользуются клиенты и какие устройства предпочитают платящие пользователи, изучу рекламные источники привлечения и определите каналы, из которых пришло больше всего платящих пользователей.  
Затем посчитаю общую сумму расходов на маркетинг, выясню как траты распределены по рекламным источникам, то есть сколько денег потратили на каждый источник, построю визуализацию динамики изменения расходов во времени по каждому источнику, узнаю сколько в среднем стоило привлечение одного пользователя (CAC) из каждого источника.  
Проведу исследование по оценки окупаемости рекламы, которое поможет ответить на вопросы: "Окупается ли реклама, направленная на привлечение пользователей в целом?", "Какие устройства, страны и рекламные каналы могут оказывать негативное влияние на окупаемость рекламы?",  "Чем могут быть вызваны проблемы окупаемости?".
На основании проведенного исследования выделю причины неэффективности привлечения пользователей и сформулирую рекомендации для отдела маркетинга.
Все этапы исследования я дополню графиками, таблицами, выводами.

**Используемые библиотеки**  
pandas, numpy, seaborn, pyplot, datetime

**Общий вывод**  
Найдены причины убытков и неэффективность привлечения пользователей развлекательного приложения.