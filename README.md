# SQL Filters

<h2>Description</h2>
Based on the attached file the code SQL code has been made. The provided SQL code involves querying a database related to clients, borrowed books, authors, and various statistical analyses. The code demonstrates a series of SELECT queries to extract specific information from the database, such as client details, borrowing patterns, popular genres, and statistics based on client characteristics.
<br />

<h2>Languages and Utilities Used</h2>
- <b>SQL</b>

<h2>Environments Used </h2>

- <b>MySQL</b> 

<h2>Walk-through:</h2>

Display all contents of the Clients table:<br />
SELECT *<br />
FROM Client;<br />

Results: <br />
ClientId,ClientFirstName,ClientLastName,ClientDoB,Occupation<br />
1,Kaiden,Hill,2006,Student<br />
2,Alina,Morton,2010,Student<br />
3,Fania,Brooks,1983,"Food Scientist"<br />
4,Courtney,Jensen,2006,Student<br />
5,Brittany,Hill,1983,Firefighter<br />
6,Max,Rogers,2005,Student<br />
7,Margaret,McCarthy,1981,"School Psychologist"<br />
8,Julie,McCarthy,1973,Professor<br />
9,Ken,McCarthy,1974,"Securities Clerk"<br />
10,Britany,O'Quinn,1984,Violinist<br />
11,Conner,Gardner,1998,"Licensed Massage Therapist"<br />
12,Mya,Austin,1960,"Parquet Floor Layer"<br />
13,Thierry,Rogers,2004,Student<br />
14,Eloise,Rogers,1984,"Computer Security Manager"<br />
15,Gerard,Jackson,1979,"Oil Exploration Engineer"<br />
16,Randy,Day,1986,"Aircraft Electrician"<br />
17,Jodie,Page,1990,"Manufacturing Director"<br />
18,Coral,Rice,1996,"Window Washer"<br />
19,Ayman,Austin,2002,Student<br />
20,Jaxson,Austin,1999,"Repair Worker"<br />
21,Joel,Austin,1973,"Police Officer"<br />
22,Alina,Austin,2010,Student<br />
23,Elin,Austin,1962,"Payroll Clerk"<br />
24,Ophelia,Wolf,2004,Student<br />
25,Eliot,McGuire,1967,Dentist<br />
26,Peter,McKinney,1968,Professor<br />
27,Annabella,Henry,1974,Nurse<br />
28,Anastasia,Baker,2001,Student<br />
29,Tyler,Baker,1984,"Police Officer"<br />
30,Lilian,Ross,1983,"Insurance Agent"<br />
31,Thierry,Arnold,1975,"Bus Driver"<br />
32,Angelina,Rowe,1979,Firefighter<br />
33,Marcia,Rowe,1974,"Health Educator"<br />
34,Martin,Rowe,1976,"Ship Engineer"<br />
35,Adeline,Rowe,2005,Student<br />
36,Colette,Rowe,1963,Professor<br />
37,Diane,Clark,1975,"Payroll Clerk"<br />
38,Caroline,Clark,1960,Dentist<br />
39,Dalton,Clayton,1982,"Police Officer"<br />
40,Steve,Clayton,1990,"Bus Driver"<br />
41,Melanie,Clayton,1987,"Computer Engineer"<br />
42,Alana,Wilson,2007,Student<br />
43,Carson,Byrne,1995,"Food Scientist"<br />
44,Conrad,Byrne,2007,Student<br />
45,Ryan,Porter,2008,Student<br />
46,Elin,Porter,1978,"Computer Programmer"<br />
47,Tyler,Harvey,2007,Student<br />
48,Arya,Harvey,2008,Student<br />
49,Serena,Harvey,1978,"School Teacher"<br />
50,Lilly,Franklin,1976,Doctor<br />
51,Mai,Franklin,1994,Dentist<br />
52,John,Franklin,1999,Firefighter<br />
53,Judy,Franklin,1995,Firefighter<br />
54,Katy,Lloyd,1992,"School Teacher"<br />
55,Tamara,Allen,1963,"Ship Engineer"<br />
56,Maxim,Lyons,1985,"Police Officer"<br />
57,Allan,Lyons,1983,"Computer Engineer"<br />
58,Marc,Harris,1980,"School Teacher"<br />
59,Elin,Young,2009,Student<br />
60,Diana,Young,2008,Student<br />
61,Diane,Young,2006,Student<br />
62,Alana,Bird,2003,Student<br />
63,Anna,Becker,1979,"Security Agent"<br />
64,Katie,Grant,1977,Manager<br />
65,Joan,Grant,2010,Student<br />
66,Bryan,Bell,2001,Student<br />
67,Belle,Miller,1970,Professor<br />
68,Peggy,Stevens,1990,"Bus Driver"<br />
69,Steve,Williamson,1975,"HR Clerk"<br />
70,Tyler,Williamson,1999,Doctor<br />
71,Izabelle,Williamson,1990,"Systems Analyst"<br />
72,Annabel,Williamson,1960,Cashier<br />
73,Mohamed,Waters,1966,"Insurance Agent"<br />
74,Marion,Newman,1970,"Computer Programmer"<br />
75,Ada,Williams,1986,"Computer Programmer"<br />
76,Sean,Scott,1983,"Bus Driver"<br />
77,Farrah,Scott,1974,"Ship Engineer"<br />
78,Christine,Lambert,1973,"School Teacher"<br />
79,Alysha,Lambert,2007,Student<br />
80,Maia,Grant,1984,"School Teacher"<br />

Find First names, last names, ages and occupations of all clients:<br />
SELECT ClientFirstName, ClientLastName, (2021 - ClientDoB) AS Age, Occupation<br />
FROM Client;<br /><br />

Results:<br />
ClientFirstName,ClientLastName,Age,Occupation<br />
Kaiden,Hill,15,Student<br />
Alina,Morton,11,Student<br />
Fania,Brooks,38,"Food Scientist"<br />
Courtney,Jensen,15,Student<br />
Brittany,Hill,38,Firefighter<br />
Max,Rogers,16,Student<br />
Margaret,McCarthy,40,"School Psychologist"<br />
Julie,McCarthy,48,Professor<br />
Ken,McCarthy,47,"Securities Clerk"<br />
Britany,O'Quinn,37,Violinist<br />
Conner,Gardner,23,"Licensed Massage Therapist"<br />
Mya,Austin,61,"Parquet Floor Layer"<br />
Thierry,Rogers,17,Student<br />
Eloise,Rogers,37,"Computer Security Manager"<br />
Gerard,Jackson,42,"Oil Exploration Engineer"<br />
Randy,Day,35,"Aircraft Electrician"<br />
Jodie,Page,31,"Manufacturing Director"<br />
Coral,Rice,25,"Window Washer"<br />
Ayman,Austin,19,Student<br />
Jaxson,Austin,22,"Repair Worker"<br />
Joel,Austin,48,"Police Officer"<br />
Alina,Austin,11,Student<br />
Elin,Austin,59,"Payroll Clerk"<br />
Ophelia,Wolf,17,Student<br />
Eliot,McGuire,54,Dentist<br />
Peter,McKinney,53,Professor<br />
Annabella,Henry,47,Nurse<br />
Anastasia,Baker,20,Student<br />
Tyler,Baker,37,"Police Officer"<br />
Lilian,Ross,38,"Insurance Agent"<br />
Thierry,Arnold,46,"Bus Driver"<br />
Angelina,Rowe,42,Firefighter<br />
Marcia,Rowe,47,"Health Educator"<br />
Martin,Rowe,45,"Ship Engineer"<br />
Adeline,Rowe,16,Student<br />
Colette,Rowe,58,Professor<br />
Diane,Clark,46,"Payroll Clerk"<br />
Caroline,Clark,61,Dentist<br />
Dalton,Clayton,39,"Police Officer"<br />
Steve,Clayton,31,"Bus Driver"<br />
Melanie,Clayton,34,"Computer Engineer"<br />
Alana,Wilson,14,Student<br />
Carson,Byrne,26,"Food Scientist"<br />
Conrad,Byrne,14,Student<br />
Ryan,Porter,13,Student<br />
Elin,Porter,43,"Computer Programmer"<br />
Tyler,Harvey,14,Student<br />
Arya,Harvey,13,Student<br />
Serena,Harvey,43,"School Teacher"<br />
Lilly,Franklin,45,Doctor<br />
Mai,Franklin,27,Dentist<br />
John,Franklin,22,Firefighter<br />
Judy,Franklin,26,Firefighter<br />
Katy,Lloyd,29,"School Teacher"<br />
Tamara,Allen,58,"Ship Engineer"<br />
Maxim,Lyons,36,"Police Officer"<br />
Allan,Lyons,38,"Computer Engineer"<br />
Marc,Harris,41,"School Teacher"<br />
Elin,Young,12,Student<br />
Diana,Young,13,Student<br />
Diane,Young,15,Student<br />
Alana,Bird,18,Student<br />
Anna,Becker,42,"Security Agent"<br />
Katie,Grant,44,Manager<br />
Joan,Grant,11,Student<br />
Bryan,Bell,20,Student<br />
Belle,Miller,51,Professor<br />
Peggy,Stevens,31,"Bus Driver"<br />
Steve,Williamson,46,"HR Clerk"<br />
Tyler,Williamson,22,Doctor<br />
Izabelle,Williamson,31,"Systems Analyst"<br />
Annabel,Williamson,61,Cashier<br />
Mohamed,Waters,55,"Insurance Agent"<br />
Marion,Newman,51,"Computer Programmer"<br />
Ada,Williams,35,"Computer Programmer"<br />
Sean,Scott,38,"Bus Driver"<br />
Farrah,Scott,47,"Ship Engineer"<br />
Christine,Lambert,48,"School Teacher"<br />
Alysha,Lambert,14,Student<br />
Maia,Grant,37,"School Teacher"<br />

Find First and last names of clients that borrowed books in March 2018:<br />
SELECT Borrower.BorrowDate, Client.ClientFirstName, Client.ClientLastName<br />
FROM Borrower<br />
INNER JOIN Client<br />
ON Borrower.ClientId = Client.ClientId<br />
WHERE Borrower.BorrowDate > "2018-02-28 00:00:00" AND Borrower.BorrowDate < "2018-04-01 00:00:00";<br /><br />

Results:<br />
BorrowDate,ClientFirstName,ClientLastName<br />
2018-03-18,Maia,Grant<br />
2018-03-18,Marcia,Rowe<br />
2018-03-07,Alysha,Lambert<br />
2018-03-11,Tyler,Baker<br />
2018-03-14,Katy,Lloyd<br />
2018-03-10,Angelina,Rowe<br />
2018-03-02,Gerard,Jackson<br />
2018-03-15,Carson,Byrne<br />

Find First and last names of the top 5 authors clients borrowed in 2017:<br />
SELECT COUNT(Borrower.BorrowId) AS CheckedOut, Author.AuthorLastName, Author.AuthorFirstName<br />
FROM Borrower<br />
INNER JOIN Book<br />
ON Borrower.BookId = Book.BookId<br />
INNER JOIN Author<br />
ON Book.BookAuthor = Author.AuthorId<br />
WHERE YEAR(Borrower.BorrowDate) = '2017'<br />
GROUP BY Author.AuthorLastName, AuthorFirstName<br />
ORDER BY CheckedOut DESC<br />
LIMIT 5;<br /><br />

Results:<br />
CheckedOut,AuthorLastName,AuthorFirstName<br />
7,Smith,Sofia<br />
7,Martin,Elena<br />
7,Moore,Logan<br />
6,Brown,Maria<br />
5,Roy,Zoe<br />

Find Nationalities of the least 5 authors that clients borrowed during the years 2015-2017:<br />
SELECT COUNT(Borrower.BorrowId) AS CheckedOut, Author.AuthorNationality<br />
FROM Borrower<br />
INNER JOIN Book<br />
ON Borrower.BookId = Book.BookId<br />
INNER JOIN Author<br />
ON Book.BookAuthor = Author.AuthorId<br />
WHERE YEAR(Borrower.BorrowDate) = '2017' OR '2016' OR '2015'<br />
GROUP BY Author.AuthorNationality<br />
ORDER BY CheckedOut<br />
LIMIT 5;<br /><br />

Results<br />
CheckedOut,AuthorNationality<br />
3,Spain<br />
8,China<br />
12,"Great Britain"<br />
21,Brazil<br />
27,France<br />

Find the book that was most borrowed during the years 2015-2017<br />
SELECT COUNT(Borrower.BorrowId) AS CheckedOut, Book.BookTitle<br />
FROM Borrower<br />
INNER JOIN Book<br />
ON Borrower.BookId = Book.BookId<br />
INNER JOIN Author<br />
ON Book.BookAuthor = Author.AuthorId<br />
WHERE YEAR(Borrower.BorrowDate) = '2017' OR '2016' OR '2015'<br />
GROUP BY Book.BookTitle<br />
ORDER BY CheckedOut DESC<br />
LIMIT 1;<br /><br />

Results:<br />
CheckedOut,BookTitle<br />
18,"Electrical transformers"<br />

Find the Top borrowed genres for client born in years 1970-1980:<br />
SELECT COUNT(Borrower.BorrowId) AS CheckedOut, Book.Genre<br />
FROM Borrower<br />
INNER JOIN Book<br />
ON Borrower.BookId = Book.BookId<br />
INNER JOIN Client<br />
ON Borrower.ClientId = Client.ClientId<br />
WHERE Client.ClientDoB BETWEEN '1969' AND '1981'<br />
GROUP BY Book.Genre<br />
ORDER BY CheckedOut DESC<br /><br />

Results:<br />
CheckedOut,Genre<br />
26,Science<br />
16,Fiction<br />
15,"Well being"<br />
5,Humor<br />
4,Society<br />
3,History<br />
3,Law<br />
3,Children<br />
3,Literature<br />

Find the Top 5 occupations that borrowed the most in 2016:<br />
SELECT COUNT(Borrower.BorrowId) AS CheckedOut, Client.Occupation<br />
FROM Borrower<br />
INNER JOIN Book<br />
ON Borrower.BookId = Book.BookId<br />
INNER JOIN Client<br />
ON Borrower.ClientId = Client.ClientId<br />
WHERE YEAR(Borrower.BorrowDate) = '2016'<br />
GROUP BY Client.Occupation<br />
ORDER BY CheckedOut DESC<br />
LIMIT 5;<br /><br />

Results<br />
CheckedOut,Occupation<br />
32,Student<br />
8,"Bus Driver"<br />
6,Dentist<br />
6,"Computer Programmer"<br />
5,"Police Officer"<br />

Find the average number of borrowed books by job title:<br />
WITH Table1 AS (SELECT COUNT(Client.ClientId) AS PeopleWJob, Client.Occupation<br />
FROM Client<br />
GROUP BY Client.Occupation),<br />
     Table2 AS (SELECT COUNT(Borrower.BorrowId) AS CheckedOut, Client.Occupation<br />
FROM Borrower<br />
INNER JOIN Book<br />
ON Borrower.BookId = Book.BookId<br />
INNER JOIN Client<br />
ON Borrower.ClientId = Client.ClientId<br />
GROUP BY Client.Occupation<br />
ORDER BY CheckedOut DESC)<br />
SELECT Table1.Occupation, (Table2.CheckedOut / Table1.PeopleWJob) AS AverageBorrows<br />
FROM Table1<br />
JOIN Table2<br />
ON Table1.Occupation = Table2.Occupation<br />
ORDER BY AverageBorrows DESC;<br /><br />

Results:<br />
Occupation,AverageBorrows<br />
Nurse,7.0000<br />
"Computer Security Manager",6.0000<br />
Dentist,5.6667<br />
"Computer Programmer",5.6667<br />
"Oil Exploration Engineer",5.0000<br />
"Manufacturing Director",5.0000<br />
Cashier,5.0000<br />
"Police Officer",4.5000<br />
Violinist,4.0000<br />
"Insurance Agent",4.0000<br />
"Bus Driver",4.0000<br />
Doctor,4.0000<br />
"HR Clerk",4.0000<br />
"Systems Analyst",4.0000<br />
Student,3.8182<br />
"School Teacher",3.6000<br />
Professor,3.5000<br />
Firefighter,3.2500<br />
"Repair Worker",3.0000<br />
"Payroll Clerk",3.0000<br />
"Computer Engineer",3.0000<br />
Manager,3.0000<br />
"Ship Engineer",2.6667<br />
"Food Scientist",2.5000<br />
"School Psychologist",2.0000<br />
"Securities Clerk",2.0000<br />
"Licensed Massage Therapist",2.0000<br />
"Parquet Floor Layer",2.0000<br />
"Aircraft Electrician",2.0000<br />
"Window Washer",2.0000<br />
"Health Educator",2.0000<br />
"Security Agent",2.0000<br />

Create a VIEW and display the titles that were borrowed by at least 20% of clients:<br />
CREATE VIEW MostPopularBooks AS <br />
SELECT Book.BookTitle, COUNT(Client.ClientId) AS CheckOuts<br />
FROM Borrower<br />
JOIN Book<br />
ON Book.BookId = Borrower.BookId<br />
JOIN Client<br />
ON Borrower.ClientId = Client.ClientId<br />
GROUP BY Book.BookTitle<br />
HAVING CheckOuts >= <br />
(SELECT (COUNT(Client.ClientId) * 0.2) AS 20pctOfClients<br />
FROM Client);<br /><br />

Results:<br />
BookTitle,CheckOuts<br />
"Electrical transformers",18<br />

Find the top month of borrows in 2017:<br />
SELECT COUNT(Borrower.BorrowId) AS NumberBorrows, MONTH(Borrower.BorrowDate) AS TopMonth2017<br />
FROM Borrower<br />
WHERE YEAR(Borrower.BorrowDate) = '2017'<br />
GROUP BY TopMonth2017<br />
HAVING NumberBorrows = <br />
(SELECT MAX(SubTable1.CheckedOut)<br />
FROM<br />
(SELECT COUNT(Borrower.BorrowId) AS CheckedOut<br />
FROM Borrower<br />
WHERE YEAR(Borrower.BorrowDate) = '2017'<br />
GROUP BY MONTH(BorrowDate)) SubTable1);<br /><br />

Results:<br />
NumberBorrows,TopMonth2017<br />
10,8<br />
10,7<br />
10,10<br />


Summary:  <br/>
The SQL code provides an extensive analysis of a database containing information about clients, borrowed books, authors, and various statistical insights. It encompasses a wide range of queries, from basic client information retrieval to more complex analyses, shedding light on borrowing patterns, popular genres, and statistical averages based on client characteristics. The code demonstrates a comprehensive exploration of the database, making it a valuable resource for understanding the relationships and patterns within the provided dataset.
</p>
