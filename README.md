# Client-Server-Application

Две программы (сервер и клиент) которые обмениваются сообщениями.
1.	Программы разработаны в Ubuntu 18.04
2.	Программыреализованы на языке С++
3.	Окно и элементы управления реализованы с использованием Qt5
4.	В случае возникновения ошибок, программы выводят соответствующие сообщения на экран.
5.  Программы собранны под Linux, запускаются как через терминал, так и через bash.



Сервер
Программа имеет элементы пользовательского интерфейса:
•	Поле ввода порта;
•	Кнопку "Старт";
•	Поле ввода сообщения;
•	Кнопку "Отправить сообщение";
•	Поле вывода сообщений.

Функционал:
1.	При нажатии на кнопку "Старт" программа ожидает подключение клиентов по заданному порту.
2.	При подключении клиента, сервер автоматически отправляет ему сообщение «Hello, client!».
3.	При нажатии на кнопку "Отправить сообщение" программа отправляет текст из поля ввода сообщения всем подключенным клиентам.
4.	Принимает сообщения от клиентов и выводить их в поле вывода сообщений.
5.	Поддерживает одновременное подключение нескольких клиентов.
6.	Сохраняет все служебные и полученные от клиентов сообщения в отдельном лог-файле в формате: дата время  |  ip-адрес:порт клиента/сервера  |  сообщение



Клиент
Программа должна иметь следующие элементы пользовательского интерфейса:
•	Поле ввода ip-адреса сервера;
•	Поле ввода порта сервера;
•	Кнопку "Подключиться";
•	Поле ввода сообщения;
•	Кнопку "Отправить сообщение";
•	Поле вывода сообщений.

Функционал:
1.	При нажатии на кнопку "Подключиться" программа устанавливает соединение с сервером, используя заданный ip-адрес и порт.
2.	При подключении к серверу, клиентавтоматически отправляет ему сообщение «Hello, server!».
3.	При нажатии на кнопку "Отправить сообщение" программа отправляет текст из поля ввода сообщения серверу.
4.	Принимать сообщения от сервера и выводит их в поле вывода сообщений;
5.	Проверка корректности ввода параметров ip-адреса и порта сервера.
6.  Обработку ошибок в случае, если клиент не может подключиться к серверу.

