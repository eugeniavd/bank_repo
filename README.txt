Этот проект основан на задаче прогнозирования ухода клиентов из "Бета-Банка". Мы строим модель, которая предсказывает, уйдет ли клиент из банка в ближайшее время или нет. Цель состоит в том, чтобы создать модель с высокой метрикой F1-меры, достигая значения не менее 0.59.

Описание данных
У нас есть исторические данные о поведении клиентов и расторжении договоров с банком. Набор данных содержит информацию о различных признаках клиентов, таких как возраст, пол, баланс на счете, количество продуктов банка и др. Целевой переменной является факт ухода клиента.

Методология

Я использую различные алгоритмы обучения: логистическую регрессию, дерево решений, случайный лес. 

Процесс решения задачи включает предобработку данных, выбор и обучение моделей, настройку гиперпараметров и оценку производительности модели на тестовой выборке.

Оценка модели

Я оцениваю производительность модели с помощью двух основных метрик: F1-меры и AUC-ROC. F1-мера представляет собой гармоническое среднее между точностью и полнотой, позволяя измерить сбалансированность модели. AUC-ROC измеряет способность модели разделять классы и показывает общую производительность модели.

Результат

На основе данных о поведении клиентов Бета-банка я построила модель, которая предсказывает отток клиентов. Для решения кейса я разделила данные на три выборки - для обучения, валидации результатов обучения и финального теста лучшей модели. До работы с классами не удавалось достичь необходимого уровня f1-меры - 0.59. Самая лучшая модель показывала 0.58.

Я увеличила выборку, увеличив количество данных по положительному классу в 4 раза. После этого удалось выполнить условия задачи и достичь F1-меры 0.59 на валидационной и 0.60 - на тестовой выборках.

Для лучшей модели я измерила метрику AUC-ROC, она показала отличный результат - 0.85 - это высокое качество предсказаний по сравнению со случайной моделью (0.50)