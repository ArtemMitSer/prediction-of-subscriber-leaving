# prediction-of-subscriber-leaving

## ЗАДАЧА
По активности абонентов в первый месяц их жизни требуется спрогнозировать уход абонента в ближайшее время.

## Данные:
- **general.csv** - общая информацию об абоненте (устройства, тарифные планы, канал продаж).   
- **traffic.csv** -  количество/длительность звонков (входящих и исходящих), количество смс, дата.  
- **recharge.csv** - аггрегированная по дням информация о пополнениях в привязке к абоненту.  
- **balance.csv** - информация о балансе абонентов на конец каждого дня.

**general.csv** содержит ***date_key*** -  дату активации. Требуется использовать ее на разделение на train и test, test - начиная с 13 мая.  
Ушедшие абоненты помечены единицей в переменной ***churn*** в файле **general.csv**.


## ТРЕБОВАНИЯ
### Метрика 
**ROC AUC**  
baseline: 0.83  
Дополнительно ответить на вопрос, почему ROC AUC а не другая? 

### Модельки минимум 
- CatBoost
- XGBoost
- logistic regression
- random forest
#### доп.
- Lightgbm

### 3 тетрадки 
**EDA.ipynb** - визуализация, поиск зависимостей для генерация фич.  
... и для каждого алгоритма своя тетрадка. 

### Шпаргалка:
[Открытый курс ODS](https://habr.com/ru/company/ods/blog/322626/ "Ссылка на курс")[Открытый курс ODS](https://habr.com/ru/company/ods/blog/322626/ "Ссылка на курс")
