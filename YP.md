## Сирык Максим Анатольевич

## 2.
База данных парикмахерской, в которую входит 6 таблиц:
*1)Appointment(Назначения);
*2)Clients(Данные о клиентах);
*3)Employees(Данные о сотрудниках);
*4)Feedback(Отзывы);
*5)Payments(Оплата);
*6)Services(Данные о стрижках).

## 2.1
	Таблица Appointments, содержащая атрибуты:
1)AppointmentID(Айди назначения, настроен по умолчанию, int);
2)DateTime(График работы, date);
3)ClientID(Айди клиента, int);
4)EmployeeID(Айди сотрудников, int);
5)ServiceID(Айди сервиса, int).
![](screens/Appointments1.png)		![](screens/Appointments2.png)

	Таблица Сlients содержащая атрибуты:
1)ClientID(Айди клиента, настроен по умолчанию, int);
2)Name(Имя, varchar(255));
3)Surname(Фамилия, varchar(255);
4)PhoneNumber(Номер телефона, varchar(255));
5)Email(Эл. почта, varchar(255));
6)Gender(Пол, varchar(255)).

	Таблица Employees содержащая атрибуты:
1)EmployeeID(Айди сотрудника, настроен по умолчанию, int);
2)Name(Имя, varchar(255));
3)Surname(Фамилия, varchar(255);
4)PhoneNumber(Номер телефона, varchar(255));
5)Email(Эл. почта, varchar(255));
6)Schedule(График работы, varchar(255));
7)Gender(Пол, varchar(255)).

	Таблица Feedback содержащая атрибуты:
1)FeedbackID(Айди отзыва, настроен по умолчанию, int);
2)ClientID(Айди клиента, int);
3)ReviewText(Текст, text);
4)Rating(Рейтинг, int).

	Таблица Payments содержащая атрибуты:
1)PaymentID(Айди оплаты, настроен по умолчанию, int);
2)FeedbackID(Айди отзыва, int);
3)PaymentAmount(Сумма к оплате, decimal(10,2));
4)PaymentDateTime(Дата оплаты, date).

	Таблица Services содержащая атрибуты:
1)ServiceID(Айди стрижки, настроен по умолчанию, int);
2)Description(Описание, text);
3)Price(Стоимость, decimal(10,2));
4)EmployeeID(Айди сотрудника, int).