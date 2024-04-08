# Аналитика ДТП
Заказчиком выступает проект [«Карта ДТП»](https://dtp-stat.ru/) — некоммерческий проект, посвященный проблеме дорожно-транспортных происшествий в России.

## Данные

Заказчик на своем сайте предоставил данные о дорожно-транспортных происшествиях в 85 регионах России за период с 2015 по 2024 годы в формате json.

## Задача 
- Провести исследовательский анализ данных о дорожно-транспортных происшествиях (ДТП).
- Сформулировать и проверить гипотезы, основываясь на имеющихся признаках.
- Построить дашборд 

## Используемые библиотеки
- pandas
- json
- dill (pickle)
- requests
- os
- google.colab 
- re
- matplotlib.pyplot
- tqdm 
- warnings
- time 
  

## Выводы. Сформировали и проверили гипотезы:
- В большинстве случаев виноваты пьяные водители, нужно усилить контроль:
  - количество ДТП с участием хотя бы одно водителя в состоянии опьянения происходят примерно в 9 раз реже, чем ДТП, где оба водителя трезвые. **Предположение, что в большинстве случаев виноваты пьяные водители не пнаходит подтверждения**
  - проверены и подтверждены гипотезы, что ДТП , в котором хотя бы один из участников находится в состоянии алкогольного опьянения, приводят к большему количеству погибших и к больг=шему количеству травмированных и раненых
- Безопасность на дорогах растет для каждого из участников:
  - Проведенные тесты отвергают гипотезы о том, что Среднее число погибших / пострадавших в ДТП в 2021-2023 годах не больше , чем среднее число погибших / пострадавших  в ДТП в 2018-2020 годах То есть люди в 2021-2023 годах погибают /получают травмы и ранения в ДТП НЕ РЕЖЕ, чем в 2018-2020 годах. Следовательно, безопасность на дорогах не растет, **проверяемая гипотеза не находит подтверждения**
- В личном автомобиле ехать безопаснее чем в автобусе:
  - Проведенные тесты отвергают нулевую гипотезу о том, что Среднее погибших в ДТП с автомобилями не больше , чем среднее погибших в ДТП с автобусами. Мы не можем подтвердить, что в автомобиле ехать безопаснее, чем в автобусе. **Проверяемая гипотеза не находит подтверждения**
- Если пешеходы не будут нарушать, то не будут гибнуть
  - Проведенные тесты отвергают гипотезу о том, что Среднее число НЕ погибших пешеходов, которые не нарушили ПДД не больше , чем среднее число НЕ погибших пешеходов, которые нарушили ПДД. То есть Пешеход меньше (реже) погибает, если не нарушает ПДД. Или же Пешеход больше (чаще) не погибает, если не нарушает ПДД. **Проверяемая гипотеза находит подтверждение**
- Низкая скорость не влияет на тяжесть ДТП
  - Проведенные тесты отвергают нулевую гипотезу о том, что Среднее число НЕ погибших людей, в ДТП, где не нарушили скоростной режим не больше , чем среднее число НЕ погибших людей, в ДТП, где нарушили скоростной режим. То есть люди меньше (реже) погибает, если не нарушается скоростной режим. Или же люди больше (чаще) не погибают, если не нарушается скоростной режим. **Проверяемая гипотеза находит подтверждение**

## Рекомендации:
- Целесообразно использовать встроенный обновляемый классификатор, который автоматически отнести бренд/модель легкового (и иного) автомобиля в соответствующую категорию.
- Целесообразно унифицировать классификацию автобусов в плане этажности
- Проверить корректность наименования и заполнения значений категорий участников  "Все участники".

##  [Ссылка на дашборд](https://datalens.yandex/s1rbmtass104g)





