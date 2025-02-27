## <center> Прогнозирование продаж товаров сети Favorita </center>
### Описание проекта

Этот проект посвящен прогнозированию временного ряда продаж различных товаров, реализуемых в магазинах Favorita в Эквадоре.

#### Этапы решения задачи:

1. Знакомство с данными – загрузка и предварительный анализ.

2. Анализ характеристик временного ряда – исследование сезонности, трендов и стационарности данных. Нахождение закономерностей и лаговых зависимостей.

3. Baseline модель (MA - Moving Average) – построение базового прогноза.

4. Линейная регрессия – предсказание с использованием модели LinearRegression.

5. ARIMA – применение авторегрессионной интегрированной модели скользящего среднего.

6. Прогнозирование с использованием Prophet – анализ временного ряда с помощью библиотеки Facebook Prophet.

7. Прогнозирование с помощью градиентных бустингов XGBoost и CatBoost – применение методов машинного обучения.

8. Сравнительный анализ моделей и выбор оптимального алгоритма – оценка точности предсказаний.

**Используемые библиотеки:**
* numpy, pandas – работа с данными
* matplotlib, plotly – визуализация
* statsmodels – статистический анализ временных рядов
* sklearn – машинное обучение
* prophet – прогнозирование временных рядов
* xgboost, catboost – градиентные бустинги

**Метрики оценки моделей:**
* MSE (Mean Squared Error)
* MAE (Mean Absolute Error)
* MAPE (Mean Absolute Percentage Error)
* RMSE (Root Mean Squared Error)

### Выводы:
По результатам тестирования различных моделей на основе временного ряда продаж были выявлены сильные и слабые стороны каждого метода:

1) Линейная регрессия показала хорошие результаты при использовании лагов, но плохо справляется с нелинейными зависимостями.

2) ARIMA работает хорошо на краткосрочных прогнозах, но требует сложной настройки гиперпараметров.

3) Prophet хорошо моделирует тренды и сезонность, но иногда переобучается или недообучается.

4) Градиентные бустинги (XGBoost, CatBoost) продемонстрировали неплохие результаты, особенно при добавлении дополнительных регрессоров (транзакции, праздники и др.).

Предлагаю вам познакомиться с [проектом](https://nbviewer.org/github/YaroslavaVob/Time-Series_project/blob/12d07fe7cfeef15c7fd34675d1ba67c302e46265/Sales%20time%20serie%20Favorita.ipynb).

Загрузить основные данные можно по [ссылке](https://drive.google.com/file/d/1i2WS6RQo32syz1DUIPdo5bdaSM_XcJq_/view?usp=sharing)

**Проект создан на базе языка Python в Jupyter Notebook.**

Автор: Ярослава Вобшаркян\
(студент школы SkillFactory по курсу Data Science)

