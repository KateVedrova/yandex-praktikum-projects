# Промышленность
Чтобы оптимизировать производственные расходы, металлургический комбинат ООО «Так закаляем сталь» решил уменьшить потребление электроэнергии на этапе обработки стали. 
Мне предстоит построить модель, которая предскажет температуру стали.
### Описание этапа обработки
Сталь обрабатывают в металлическом ковше вместимостью около 100 тонн. Чтобы ковш выдерживал высокие температуры, изнутри его облицовывают огнеупорным кирпичом. 
Расплавленную сталь заливают в ковш и подогревают до нужной температуры графитовыми электродами. Они установлены в крышке ковша.\
Из сплава выводится сера (десульфурация), добавлением примесей корректируется химический состав и отбираются пробы. 
Сталь легируют — изменяют её состав — подавая куски сплава из бункера для сыпучих материалов или проволоку через специальный трайб-аппарат (англ. tribe, «масса»).\
Перед тем как первый раз ввести легирующие добавки, измеряют температуру стали и производят её химический анализ. 
Потом температуру на несколько минут повышают, добавляют легирующие материалы и продувают сплав инертным газом. Затем его перемешивают и снова проводят измерения. 
Такой цикл повторяется до достижения целевого химического состава и оптимальной температуры плавки. 
Тогда расплавленная сталь отправляется на доводку металла или поступает в машину непрерывной разливки. Оттуда готовый продукт выходит в виде заготовок-слябов (англ. slab, «плита»).
### Описание данных
Данные состоят из файлов, полученных из разных источников:
- data_arc_new.csv — данные об электродах;
- data_bulk_new.csv — данные о подаче сыпучих материалов (объём);
- data_bulk_time_new.csv — данные о подаче сыпучих материалов (время);
- data_gas_new.csv — данные о продувке сплава газом;
- data_temp_new.csv — результаты измерения температуры;
- data_wire_new.csv — данные о проволочных материалах (объём);
- data_wire_time_new.csv — данные о проволочных материалах (время).
###  Используемые библиотеки:
- matplotlib.pyplot;
- numpy; 
- pandas;
- seaborn; 
- catboost; 
- sklearn.
### Вывод:
Была выбрана модель CatBoostRegressor с гиперпараметрами:

random_state= 110923,
verbose=False,
learning_rate=0.05,
max_depth=3,
n_estimators=500
