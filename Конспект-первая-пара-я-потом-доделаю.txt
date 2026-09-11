== ПЕРВАЯ ПАРА ==

компьютер -> сервер (экземпляр) -> бд (часть экземпляра) -> таблицы -> данные

типы данных БД
1. битовые
2. целочисленные (int)
3. дробные (real, float, decimal)
4. символьные (char, varchar, nvarchar)
	varchar - ascii
	nvarchar - unicode
5. дата и время (datetime, smalldatetime)
6. специальные (text, bit - boolean, image)
7. денежные (money)

расширения:
1. mdf - база
2. ldf - логи

tempdf - временная бд

состав бд:
1. таблицы
2. представления - набор данных
3. хранимые процедурые
4. BLOB-поля: данные в формате больших двоичных данных
5. метаданные

системные бд:
1. master - главная бд сервера, хранит инфу о пользователях, настройки, инфу о бд и др.
2. model - шаблон для создания бд
3. msdb - информация о выполняемой работе (команды, бэкапы)
4. tempdb - хранилище временных объектов


sql server 2025 + ms SQL server managment studio
1. создаём сервер в sql server-> подключаемся к нему в ms sql server managment
2. создаём бд внутри экземпляра сервера (нужны права админа...)
3. создаём таблицу
	пример: 
USE [college] 
GO

CREATE TABLE [dbo].[Users] ( 
	[Id] INT IDENTITY(1,1) PRIMARY KEY,
	[Login] NVARCHAR(50) NOT NULL UNIQUE,
	[Age] INT NOT NULL
	);

GO
4. создаём ряды (через боль)












