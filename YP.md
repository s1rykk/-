## Сирык Максим Анатольевич

## 2.
База данных парикмахерской, в которую входит 6 таблиц:
* Appointment(Назначения);
* Clients(Данные о клиентах);
* Employees(Данные о сотрудниках);
* Feedback(Отзывы);
* Payments(Оплата);
* Services(Данные о стрижках).

## 2.1
	Таблица Appointments, содержащая атрибуты:
* AppointmentID(Айди назначения, настроен по умолчанию, int);
* DateTime(График работы, date);
* ClientID(Айди клиента, int);
* EmployeeID(Айди сотрудников, int);
* ServiceID(Айди сервиса, int).

![](screens/Appointments1.png)		![](screens/Appointments2.png)

	Таблица Сlients содержащая атрибуты:
* ClientID(Айди клиента, настроен по умолчанию, int);
* Name(Имя, varchar(255));
* Surname(Фамилия, varchar(255);
* PhoneNumber(Номер телефона, varchar(255));
* Email(Эл. почта, varchar(255));
* Gender(Пол, varchar(255)).

![](screens/Clients1.png)		![](screens/Clients2.png)

	Таблица Employees содержащая атрибуты:
* EmployeeID(Айди сотрудника, настроен по умолчанию, int);
* Name(Имя, varchar(255));
* Surname(Фамилия, varchar(255));
* PhoneNumber(Номер телефона, varchar(255));
* Email(Эл. почта, varchar(255));
* Schedule(График работы, varchar(255));
* Gender(Пол, varchar(255)).

![](screens/Employees1.png)		![](screens/Employees2.png)

	Таблица Feedback содержащая атрибуты:
* FeedbackID(Айди отзыва, настроен по умолчанию, int);
* ClientID(Айди клиента, int);
* ReviewText(Текст, text);
* Rating(Рейтинг, int).

![](screens/Feedback1.png)		![](screens/Feedback2.png)

	Таблица Payments содержащая атрибуты:
* PaymentID(Айди оплаты, настроен по умолчанию, int);
* FeedbackID(Айди отзыва, int);
* PaymentAmount(Сумма к оплате, decimal(10,2));
* PaymentDateTime(Дата оплаты, date).

![](screens/Payments1.png)		![](screens/Payments2.png)

	Таблица Services содержащая атрибуты:
* ServiceID(Айди стрижки, настроен по умолчанию, int);
* Description(Описание, text);
* Price(Стоимость, decimal(10,2));
* EmployeeID(Айди сотрудника, int).

![](screens/Services.png)		![](screens/Services2.png)


## 3. Демонстрация работы функции UNION
Объединение двух наборов строк. Я объединил Name и Surname из таблицы Clients.
![](screens/UNION.png)


## 4. Демонстрация работы функции ORDER BY
Сортировка данных. Я отсортировал стоимость стрижки по возрастанию.
![](screens/ORDER_BY.png)


## 5. Демонстрация работы функции HAVING
Я отфильтровал результаты, где стоимость стрижки больше 25.

![](screens/SELECT.png)


## 6. Демонстрация работы вложенных запросов
### 6.1. В SELECT
Вывел клиента, чье имя Дима из таблицы Клиентов

![](screens/SELECT.png)

### 6.1. В WHERE
