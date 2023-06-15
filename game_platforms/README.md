# Исследование данных о продаже игр, оценках пользователей и экспертов, жанрах и платформах  

**Описание данных:**  
Датафрейм games:   
* name — название игры;  
* platform — платформа;  
* year_of_release — год выпуска;  
* genre — жанр игры;  
* na_sales —  продажи в Северной Америке (миллионы проданных копий);  
* eu_sales — продажи в Европе (миллионы проданных копий); 
* jp_sales — продажи в Японии (миллионы проданных копий);
* other_sales — продажи в других странах (миллионы проданных копий);
* critic_score — оценка критиков (максимум 100);
* user_score — оценка пользователей (максимум 10);
* rating — рейтинг от организации ESRB (англ. Entertainment Software Rating Board). Эта ассоциация определяет рейтинг компьютерных игр и присваивает им подходящую возрастную категорию.  

**Цель исследования:**
выявить закономерности определяющие успешность игры.

**Задачи исследования:**  
1. Привести в необходимый вид данные для проведения анализа.  
2. Посчитать и добавить в таблицу дополнительные данные для дальнейшего изучения.  
3. Определить какие платформы лидируют по продажам, растут или падают?  
4. Проанализировать влияние отзывов пользователей и критиков на продажи внутри одной популярной платформы.  
5. Определить самые прибыльные жанры игр.
6. Составить портрет пользователя каждого региона.  
7. Проверить гипотезы:  
   * Средние пользовательские рейтинги платформ Xbox One и PC одинаковые;  
   * Средние пользовательские рейтинги жанров Action и Sports разные.

**Ход исследования:**  
Данные для проведения исследования я возьму из файла — '/datasets/games.csv'. В начале исследования данные из файла необходимо проверить на пропуски, анамалии, ошибки, дубликаты. Затем дополню имеющуюся информацию дополнительными расчетами. На основании всех полученных данных я проведу исследование, которое поможет ответить на вопросы: "Какие платформы лидируют по продажам, растут или падают?", "Какое влияние оказывают отзывы пользователей и критиков на продажи внутри одной популярной платформы?", "Какие самые прибыльные жанры игр?". А также поможет составить портрет пользователя каждого региона, а также проверить выдвинутые гипотизы.
Все этапы исследования я дополню графиками, таблицами, выводами.

**Используемые библиотеки**  
pandas, numpy, matplotlib, scipy