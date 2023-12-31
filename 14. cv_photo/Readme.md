# 14. Определение возраста покупателей по фото.

## Данные:

Набор фотографий людей с указанием возраста:

 - Фото людей 
 - Метка с указанием возраста людей на фото

## Задачи проекта:

 - Построим модель, которая по фотографии определит приблизительный возраст человека.
 - Ключевой метрикой качества модели является МАЕ, которая должна быть не более 8.

## Используемые библиотеки:
 - Python ver.3
 - Pandas
 - Numpy
 - PIL
 - Matplotlib
 - Tensorflow

## Выводы:
 - Для решения поставленной задачи использовалась модель архитектуры ResNet c 50 слоями.
 - Решалась задача регрессии, то есть модель предсказывала число(возраст по фото), поэтому выходной нейрон 1.
 - При этом оптимальной было использование функции активации "ReLU", которая не меняет положительные прогнозы, а отрицательные приводит к нулю.
 - Тестовый показатель MAE составил 5.88, что лучше максимально заявленных для решения задачи 8.
 - Разница в МАЕ на тестовой и обучающей выборках существенна, почти в 2 раза. Но переобучения не случилось, задача выполнена.
 - Данные по возрастам распределены не однородно, возможно если произвести более подробную подготовку изображений, то показатель мог быть улучшен.