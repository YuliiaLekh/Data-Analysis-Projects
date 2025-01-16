Опис даних
Джерело
Дані взяті з Kaggle за посиланням Rossmann Store Sales. https://www.kaggle.com/competitions/rossmann-store-sales/data

Основні характеристики
Продажі за день для магазинів Rossmann.
Інформація про магазини: тип, конкуренція, промоції.
Часові дані: дата, день тижня.
Додаткові параметри: святкові дні, шкільні канікули.
Формат даних: CSV-файли з інформацією про магазини та продажі.
Available Files
train.csv: Historical data including Sales.
test.csv: Historical data excluding Sales.
sample_submission.csv: A sample submission file in the correct format.
store.csv: Supplemental information about the stores.
Data Fields
General Information
Id: An identifier representing a (Store, Date) duple within the test set.
Store: A unique identifier for each store.
Sales: The turnover for any given day (this is the target variable for prediction).
Customers: The number of customers visiting on a given day.
Open: Indicates whether the store was open:
0: Closed
1: Open
StateHoliday: Indicates a state holiday. Normally, all stores (with few exceptions) are closed:
a: Public holiday
b: Easter holiday
c: Christmas
0: None (not a holiday)
SchoolHoliday: Indicates if the (Store, Date) was affected by the closure of public schools:
0: No school holiday
1: School holiday
Store Characteristics
StoreType: Differentiates between 4 types of store models:
a, b, c, d
Assortment: Describes the level of assortment:
a: Basic
b: Extra
c: Extended
CompetitionDistance: Distance in meters to the nearest competitor store.
CompetitionOpenSince[Month/Year]: Approximate month and year when the nearest competitor store was opened.
Promotional Information
Promo: Indicates if a store is running a promotion on that day:
0: No promotion
1: Promotion running
Promo2: Indicates if the store is participating in Promo2, a continuous promotion:
0: Store is not participating
1: Store is participating
Promo2Since[Year/Week]: The year and calendar week when the store started participating in Promo2.
PromoInterval: Describes the months when Promo2 starts anew for a store. For example:
"Feb,May,Aug,Nov": Promo2 starts in February, May, August, and November of each year.
2. Формулювання запитань
Головне питання:
Які чинники найбільше впливають на обсяг продажів?
Додаткові запитання:
Як впливає кількість клієнтів на обсяг продажів?
Чи спостерігаються сезонні тренди у продажах (щомісячно, щорічно)?
Як змінюється продаж залежно від типу магазину (StoreType)?
Чи впливають дні тижня на обсяг продажів?
Який вплив має реклама (Promo) на продажі?
Чи є різниця у продажах під час святкових днів (StateHoliday)?
Який вплив має щільність клієнтів (Sales/Customers)?
Чи існує кореляція між розміром магазину (CompetitionDistance) і продажами?
Як на продажі впливає участь у шкільних канікулах (SchoolHoliday)?
Як зміна в промоціях (Promo, Promo2) впливає на кількість клієнтів (Customers)?
Який вплив має тип асортименту (Assortment) на продажі?
Як тип асортименту (Assortment) впливає на середній обсяг продажів у різних типах магазинів (StoreType)?
Як впливає участь у промоціях (Promo та Promo2) на середній обсяг продажів у різні місяці року?
