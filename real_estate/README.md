# Исследование объявлений о продаже квартир

Исследование проводится в интересах сервиса Яндекс Недвижимость. На основании архива объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах за несколько лет следует научиться определять рыночную стоимость объектов недвижимости.

***Ограничения исследования:***

1. По каждой квартире на продажу доступны два вида данных  
Первые вписаны пользователем, вторые — получены автоматически на основе картографических данных

 
***Цель исследования:***

1. Определить рыночную стоимость объектов недвижимости
2. Установить, какие факторы влияют на ценообразование стоимости квартир

***Ход исследования***

Данные о недвижимости я получу из файла "...datasets/real_estate_data.csv". О качестве данных ничего не известно. Поэтому перед тем, как приступать к целям исследования, понадобится обзор данных

Я проверю данные на ошибки и оценю их влияние на исследование. Затем, на этапе предобработки я поищу возможность исправить все ошибки данных, которые не приведут к искажению конечного результата. Далее, создам необходимые столбцы, и приступлю к проведению исследовательского анализа

Таким образом, моё исследование пройдёт в пять этапов:

* Обзор данных
* Предобработка данных
* Расчеты и добавление результатов в таблицу
* Проведение анализа исследовательского анализа для Санкт-Петербурга и Ленинградской области
* Написание общего вывода

***Описание данных***
 - airports_nearest — расстояние до ближайшего аэропорта в метрах (м)
 - balcony — число балконов
 - ceiling_height — высота потолков (м)
 - cityCenters_nearest — расстояние до центра города (м)
 - days_exposition — сколько дней было размещено объявление (от публикации до снятия)
 - first_day_exposition — дата публикации
 - floor — этаж
 - floors_total — всего этажей в доме
 - is_apartment — апартаменты (булев тип)
 - kitchen_area — площадь кухни в квадратных метрах (м²)
 - last_price — цена на момент снятия с публикации
 - living_area — жилая площадь в квадратных метрах (м²)
 - locality_name — название населённого пункта
 - open_plan — свободная планировка (булев тип)
 - parks_around3000 — число парков в радиусе 3 км
 - parks_nearest — расстояние до ближайшего парка (м)
 - ponds_around3000 — число водоёмов в радиусе 3 км
 - ponds_nearest — расстояние до ближайшего водоёма (м)
 - rooms — число комнат
 - studio — квартира-студия (булев тип)
 - total_area — общая площадь квартиры в квадратных метрах (м²)
 - total_images — число фотографий квартиры в объявлении