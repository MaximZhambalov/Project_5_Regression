![](./images/taximeter.jpg)
# <center> Проект 4: Классификация клиентов банка </center>

## Оглавление
1. [Описание проекта](#Описание-проекта)
2. [Описание данных](#Описание-данных)
3. [Зависимости](#Зависимости)
4. [Установка проекта](#Установка-проекта)
5. [Использование проекта](#Использование-проекта)
6. [Выводы](Использование-проекта)

## Описание проекта

**Данный проект** выполнен в рамках учебного курса с целью попрактиковаться решать задачи регрессии.

**О структуре проекта:**
* [images](./images) - папка с изображениями, необходимыми для проекта.
* [data](./data) - папка с данными.
* [Project-5-Regression.ipynb](./Project-5-Regression.ipynb) - jupyter-ноутбук, содержащий основной код проекта: чтение и обработкеа данных, преобразование данных и моделирование.


## Описание данных
Нам предстоит решить задачу машинного обучения, направленную на автоматизацию бизнес процессов. Мы построим модель, которая будет предсказывать общую продолжительность поездки такси в Нью-Йорке. 

Представьте, что вы заказываете такси из одной точки Нью-Йорка в другую, причем не обязательно конечная точка должна находиться в пределах города. Сколько вы должны будете за нее заплатить? Известно, что стоимость такси в США рассчитывается на основе фиксированной ставки + тарифная стоимость, величина которой зависит от времени и расстояния. Тарифы варьируются в зависимости от города.

В свою очередь время поездки зависит от множества факторов таких как, откуда и куда вы едете, в какое время суток вы совершаете вашу поездку, погодных условий и так далее. 

Таким образом, если мы разработаем алгоритм, способный определять длительность поездки, мы сможем прогнозировать ее стоимость самым тривиальным образом, например, просто умножая стоимость на заданный тариф. 
Сервисы такси хранят огромные объёмы информации о поездках, включая такие данные как конечная, начальная точка маршрута, дата поездки и ее длительность. Эти данные можно использовать для того, чтобы прогнозировать длительность поездки в автоматическом режиме с привлечением искусственного интеллекта.

**Бизнес-задача:** определить характеристики и с их помощью спрогнозировать длительность поездки такси.

**Техническая задача:** построить модель машинного обучения, которая на основе предложенных характеристик клиента будет предсказывать числовой признак - время поездки такси, то есть решить задачу регрессии.

**Основные цели проекта:**
1. Сформировать набор данных на основе нескольких источников информации
2. Спроектировать новые признаки с помощью *Feature Engineering* и выявить наиболее значимые при построении модели
3. Исследовать предоставленные данные и выявить закономерности
4. Построить несколько моделей и выбрать из них наилучшую по заданной метрике
5. Спроектировать процесс предсказания времени длительности поездки для новых данных

**Примечание:** Задача, которую мы будем решать, была представлена в качестве [соревнования](https://www.kaggle.com/competitions/nyc-taxi-trip-duration/overview) с призовым фондом в $30 000 $\$ на платформе *Kaggle* в 2017 году.

Нам предоставлен набор данных, содержащий информацию о поездках на жёлтом такси в Нью-Йорке за 2016 год. Первоначально данные были выпущены Комиссией по Такси и Лимузинам Нью-Йорка и включают в себя информацию о времени поездки, географических координатах, количестве пассажиров и несколько других переменных.

## Используемые зависимости
* Python (3.9):
    * [pandas (1.3.4)](https://pandas.pydata.org)
    * [numpy (1.23.5)](https://pypi.org/project/psycopg2/)
    * [seaborn (0.12.2)](https://plotly.com/python/)
    * [matplotlib (3.6.3)](https://matplotlib.org/)
    * [scikit-learn (1.2.2)](https://scikit-learn.org/stable/index.html)
    * [plotly (5.13.0)](https://plotly.com/python/plotly-express/)
    * [scipy 1.9.3](https://scipy.org/)
    * [catboost 1.2](https://catboost.ai/)
    * [xgboost 1.7.6](https://xgboost.readthedocs.io/en/stable/)

## Установка проекта
```
git clone https://github.com/MaximZhambalov/Project-5-Regression
```

## Использование
Вся информация о работе представлена в jupyter-ноутбуке Project-5-Regression.ipynb.
Часть данных, необходимых для работы ноутука находятся [здесь](https://disk.yandex.ru/d/__BHqM61m-t8kw)

## Выводы
В этом проекте:
- проведён разведовательный анализ данных, обработан и подготовлен датасет для модели;
- была построена модель, предсказывающая, откроет ли клиент счёт в банке. Финальное значение метрики ???????.