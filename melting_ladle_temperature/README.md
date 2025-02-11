# Предсказание температуры в плавильном ковше

## Описание проекта

Металлургическому заводу требуется предсказать температуру в плавильном ковше с метрикой *MAE* не хуже 6,8 °C. Предоставлены 7 таблиц с информацией о параметрах работы нагревательного устройства (электрической дуги), материалах, поступающих в ковш (сыпучие, проволочные, газ), температуре в ковше в разные моменты времени.

## Использовавшиеся библиотеки
- catboost
- numpy
- optuna
- pandas
- pandas_profiling
- seaborn
- shap
- sklearn
- matplotlib


## Что сделано
Выполнен анализ и обработка данных, сгенерированы новые признаки, обучены 3 модели машинного обучения (линейная регрессия, случайный лес, градиентный бустинг).

## Выводы
Лучший результат получен для модели градиентного бустинга (CatBoost). Значение *MAE* на тестовой выборке составило 5,3 °C.
