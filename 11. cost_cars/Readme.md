# 11. Определение стоимости автомобилей.

## Данные:

Исторические данные из сервиса по продаже автомобилей:

 - Дата скачивания анкеты из базы
 - Тип автомобильного кузова
 - Год регистрации автомобиля
 - Тип коробки передач
 - Мощность двигателя (л.с.)
 - Модель автомобиля
 - Пробег(км)
 - Месяц регистрации автомобиля
 - Тип топлива
 - Марка автомобиля
 - Была машина в ремонте или нет
 - Дата создания анкеты
 - Количество фотографий автомобиля
 - Почтовый индекс владельца анкеты(пользователя)
 - Дата последней активности пользователя
 - Цена(евро)
 
## Задачи проекта:

 - Исходя из исторических данных сервиса по продаже автомобилей построить модель, которая определит стоимость автомобиля.
 - Для решения задачи важны качество предсказания, скорость предсказания, время обучения.

## Используемые библиотеки:
 - Python ver.3
 - Pandas
 - Matplotlib
 - Seaborn
 - Numpy
 - Sklearn
 - Catboost
 - Lightgbm
 - Re
 - Time


## Выводы:
 - Модели "Градиентного бустинга" в данной задаче предсказания цены автомобиля на основе некоторых входящих данных, показали существенно лучший RMSE, чем "Линейная модель" и "Модель дерева решений".
 - Модель "Дерева-решений" "DecisionTreeRegressorr" выдала средний RMSE, но время как обучения, так и предсказания сильно быстрее остальных моделей.
 - Наилучшее RMSE и существенно более короткое время обучения показала модель "LGBMRegressor". Ее то мы и выбираем для решения задачи, как оптимальную.
 - Модель "CatBoostRegressor " имеет большой запас и потенциал, но для ее настройки и работы требуется достаточно мощный компьютер, а время предсказания у нее немного, но быстрее, чем у "LGBMRegressor".