# Предсказание стоимости автомобилей

## Статус проекта
`Завершен`

## Задача
Необходимо построить модель машинного обучения, которая сможет быстро, качественно подсказать клиенту рыночную стоимость автомобиля. Данная модель в дальнейшем будет интегрирована в приложение по продаже автомобилей с пробегом.

## Используемые библиотеки и инструменты
- pandas;
- sklearn;
- matplotlib;
- seaborn;
- numpy;
- catboost;
- lightgbm.

## Результат
Рассмотрев модели LGBMRegressor и CatBoostRegressor, можно сделать следующие выводы:

- Скорость обучения: наиболее быстрой моделью оказалась модель LGBMRegressor, которая провела обучение за чуть больше 1 минуты в то время, как вторая модель за примерно 25 минут (возможно это связано с тем, что в первом случае категориальные признаки прошли через OrdinalEncoder);
- Скорость предсказания: здесь же быстрой оказалась модель CatBoostRegressor, которая вывела ответа за 3.5 секунды в то время, как первая модель за 10 секунд;
- Качество предсказания: качество моделей примерно одинаковое, но модель CatBoostRegressor оказалась немного да точнее с RMSE, равным 1403 (это значит, что в среднем ответы отклоняются от реальных на 1403 евро), а LGBMRegressor - 1409.
