# Восстановление золота из руды
Необходимо подготовить прототип модели машинного обучения для «Цифры». Компания разрабатывает решения для эффективной работы промышленных предприятий.
Мне предстоит построить модель, которая должна предсказать коэффициент восстановления золота из золотосодержащей руды. Нужно использовать данные с параметрами добычи и очистки.
Модель поможет оптимизировать производство, чтобы не запускать предприятие с убыточными характеристиками.
### Описание данных
Данные состоят из файлов:
- gold_industry_train.csv — обучающая выборка;
- gold_industry_test.csv — тестовая выборка;
- gold_industry_full.csv — исходные данные.
###  Используемые библиотеки:
- matplotlib.pyplot;
- numpy; 
- pandas;
- sklearn.
### Вывод:
Была выбрана модель RandomForestRegressor с гиперпараметрами:

random_state= 0,
max_depth=3,
n_estimators=41

