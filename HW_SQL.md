## Complete exercise

### NORMAL level

#### Task 1 💻
На сайте w3schools.com на странице Learn SQL: http://www.w3schools.com/sql/default.asp
Нажать кнопку `Try it yourself`,  далее в новом окне нажать на кнопку  `Run SQL`
Запросы для таблицы `Customers`:
1. Вывести всех, кточто живет в Лондоне
SELECT * FROM Customers WHERE City = "London"
2. Выбрать имена контактов и имена заказчиков, где адрес заканчивается на 23
SELECT CustomerName, ContactName, Address FROM Customers WHERE Address LIKE '%23'
3. Выбрать уникальные города.
SELECT  Distinct City FROM Customers   
4. Выбрать тех пользователей, у кого код начинается с 0 (нуль)
SELECT * FROM Customers  WHERE Postalcode Like '0%'
5. Вывести клиентов не из США
SELECT * FROM Customers WHERE Country != "USA"
6. Вывести всех, кто из Франции и отсортировать по убыванию по имени контакта
SELECT * FROM Customers WHERE Country = "France"  Order by ContactName desc
7. Вывести клиентов из Германии и США, ограничить выбор 10 записями
SELECT * FROM Customers WHERE Country = "France" or "USA" limit 10

#### Task 2 💻
На сайте w3schools.com на странице Learn SQL: http://www.w3schools.com/sql/default.asp
Нажать кнопку `Try it yourself`,  далее в новом окне нажать на кнопку  `Run SQL`
Запросы для таблицы `Products`:
1. Выбрать все продукты, начинающиеся на букву «М»
SELECT * FROM Products where ProductName like 'M%'
2. Вывести характеристику упаковки (unit) для товара Steeleye Stout
SELECT Unit FROM Products where ProductName ='Steeleye Stout'
3. Вывести названия товаров, цена которых выше 22
SELECT * FROM Products where Price > 22
4. Вывести товары, в которых вес упаковки составляет 500 250 g 
 SELECT * FROM Products WHERE Unit like '%250 g%' or unit like '%500 g%'  
5. Вывести товары, упаковка которых состоит из «bottles»
 SELECT * FROM Products WHERE Unit Like '%bottles%'
6. Вывести товары, где SupplierID составляет 7 и отсортировать результаты по убыванию по цене
 SELECT * FROM Products WHERE SupplierID = '7' order by Price desc

#### Task 3 💻
На веб-странице существует кнопка `«Быстрый поиск»`, которая выделяет из таблицы `character` в базе данных всех персонажей выше 45 уровня (столбец `level`), расы dwarf(столбец `race`) и выводит результат на страницу. Укажите, как будет выглядеть в данном случае SQL-запрос.

#### Task 4 💻
На сайте w3schools.com на странице Learn SQL: http://www.w3schools.com/sql/default.asp
Нажать кнопку `Try it yourself`,  далее в новом окне нажать на кнопку  `Run SQL`
Запросы для таблицы `Employees`:
1. Вывести имя, фамилию и записи о сотруднике Leverling
SELECT FirstName, LastName,  Notes FROM Employees where lastname = 'Leverling'
2. Вывести информацию по работникам старше 1960 года
SELECT Notes FROM Employees where BirthDate > 1960
3. Вывести  дату рождения сотрудников, чьи имена начинаются на букву «А
SELECT BirthDate FROM Employees where FirstName like "A%" 
4. Вывести имя, фамилию и дату рождения сотрудников, отсортировав по дате рождения по возрастанию
SELECT FirstName, LastName , BirthDate FROM Employees order by BirthDate asc

