# LCW-SQL-ODEV

# PostgreSQL Employee Tablosu ve İşlemler

Bu döküman, SQL Ödevi kapsamında gerçekleştirilecek adımları içerir.

---

## **1. test Veritabanınızı Oluşturun**

```sql
CREATE DATABASE test;
```

---

## **2. employee Tablosunu Oluşturun**

```sql
CREATE TABLE employee (
    id SERIAL PRIMARY KEY,
    name VARCHAR(50),
    birthday DATE,
    email VARCHAR(100)
);
```

---

## **3. Mockaroo'dan Aldığınız 50 Adet Veriyi Ekleyin**

```sql
insert into employee (id, name, birthday, email) values (1, 'Glyn', '1/8/2025', 'gkinnerk0@miibeian.gov.cn');
insert into employee (id, name, birthday, email) values (2, 'Aurelea', '9/13/2024', 'apascall1@google.cn');
insert into employee (id, name, birthday, email) values (3, 'Silvanus', '3/18/2024', 'sshipperbottom2@buzzfeed.com');
insert into employee (id, name, birthday, email) values (4, 'Kerrill', '6/27/2024', 'kport3@livejournal.com');
insert into employee (id, name, birthday, email) values (5, 'Clarisse', '10/25/2024', 'canthill4@blinklist.com');
insert into employee (id, name, birthday, email) values (6, 'Giraldo', '11/19/2024', 'gpolfer5@gizmodo.com');
insert into employee (id, name, birthday, email) values (7, 'Nick', '6/13/2024', 'nredfearn6@jugem.jp');
insert into employee (id, name, birthday, email) values (8, 'Ruben', '6/14/2024', 'rleleu7@opera.com');
insert into employee (id, name, birthday, email) values (9, 'Joannes', '9/24/2024', 'jmcinnerny8@ft.com');
insert into employee (id, name, birthday, email) values (10, 'Jo-ann', '5/16/2024', 'jroebottom9@simplemachines.org');
insert into employee (id, name, birthday, email) values (11, 'Ortensia', '7/10/2024', 'opriesta@squidoo.com');
insert into employee (id, name, birthday, email) values (12, 'Dianemarie', '10/29/2024', 'dcobbb@unesco.org');
insert into employee (id, name, birthday, email) values (13, 'Jerrylee', '11/13/2024', 'jwaszkiewiczc@baidu.com');
insert into employee (id, name, birthday, email) values (14, 'Jeanne', '12/17/2024', 'jwhittingtond@etsy.com');
insert into employee (id, name, birthday, email) values (15, 'Sampson', '11/20/2024', 'sdeye@vinaora.com');
insert into employee (id, name, birthday, email) values (16, 'Bentley', '4/12/2024', 'bsawellf@ucla.edu');
insert into employee (id, name, birthday, email) values (17, 'Jill', '9/5/2024', 'jkiliang@sohu.com');
insert into employee (id, name, birthday, email) values (18, 'Brunhilda', '7/13/2024', 'bgiannassih@noaa.gov');
insert into employee (id, name, birthday, email) values (19, 'Clary', '9/14/2024', 'cmanjini@miitbeian.gov.cn');
insert into employee (id, name, birthday, email) values (20, 'Hazel', '3/15/2024', 'hhartupj@quantcast.com');
insert into employee (id, name, birthday, email) values (21, 'Shea', '10/17/2024', 'spechetk@imgur.com');
insert into employee (id, name, birthday, email) values (22, 'Guthrie', '12/10/2024', 'gbelderfieldl@engadget.com');
insert into employee (id, name, birthday, email) values (23, 'Harvey', '4/30/2024', 'hvasyuninm@icio.us');
insert into employee (id, name, birthday, email) values (24, 'Sonia', '8/16/2024', 'spasmoren@angelfire.com');
insert into employee (id, name, birthday, email) values (25, 'Edmund', '4/3/2024', 'eharsumo@shinystat.com');
insert into employee (id, name, birthday, email) values (26, 'Carlie', '3/28/2024', 'cspenderp@engadget.com');
insert into employee (id, name, birthday, email) values (27, 'Allianora', '6/27/2024', 'aaccumq@eepurl.com');
insert into employee (id, name, birthday, email) values (28, 'Thomasina', '9/13/2024', 'tbleesr@ustream.tv');
insert into employee (id, name, birthday, email) values (29, 'Sanderson', '11/22/2024', 'stippells@sfgate.com');
insert into employee (id, name, birthday, email) values (30, 'Janeczka', '4/20/2024', 'jbecclest@twitpic.com');
insert into employee (id, name, birthday, email) values (31, 'Nikolaos', '4/14/2024', 'nvanderspohru@oracle.com');
insert into employee (id, name, birthday, email) values (32, 'Kriste', '12/14/2024', 'kkildayv@issuu.com');
insert into employee (id, name, birthday, email) values (33, 'Kelsey', '3/7/2024', 'kbolinw@hud.gov');
insert into employee (id, name, birthday, email) values (34, 'Ring', '5/29/2024', 'ringersonx@barnesandnoble.com');
insert into employee (id, name, birthday, email) values (35, 'Kirby', '7/8/2024', 'khunny@mlb.com');
insert into employee (id, name, birthday, email) values (36, 'Reena', '12/6/2024', 'rborellz@nydailynews.com');
insert into employee (id, name, birthday, email) values (37, 'Gordon', '12/6/2024', 'gatthowe10@bravesites.com');
insert into employee (id, name, birthday, email) values (38, 'Jeni', '12/14/2024', 'jsutor11@tinypic.com');
insert into employee (id, name, birthday, email) values (39, 'Jerrie', '11/28/2024', 'jspeakman12@apache.org');
insert into employee (id, name, birthday, email) values (40, 'Sibilla', '11/11/2024', 'slavington13@senate.gov');
insert into employee (id, name, birthday, email) values (41, 'Gawain', '4/6/2024', 'greddy14@newsvine.com');
insert into employee (id, name, birthday, email) values (42, 'Rosabella', '6/2/2024', 'rbateman15@dedecms.com');
insert into employee (id, name, birthday, email) values (43, 'Theo', '5/3/2024', 'tmcduffie16@weather.com');
insert into employee (id, name, birthday, email) values (44, 'Bridgette', '4/1/2024', 'blucien17@columbia.edu');
insert into employee (id, name, birthday, email) values (45, 'Athene', '4/12/2024', 'ahaycox18@nymag.com');
insert into employee (id, name, birthday, email) values (46, 'Debby', '8/17/2024', 'divan19@dion.ne.jp');
insert into employee (id, name, birthday, email) values (47, 'Burl', '8/23/2024', 'bwyles1a@sakura.ne.jp');
insert into employee (id, name, birthday, email) values (48, 'Hilario', '2/3/2024', 'htrigwell1b@nasa.gov');
insert into employee (id, name, birthday, email) values (49, 'Allis', '11/21/2024', 'abroker1c@usgs.gov');
insert into employee (id, name, birthday, email) values (50, 'Brander', '12/20/2024', 'bpesterfield1d@dedecms.com');

```

---

## **4. Her Sütuna Göre Diğer Sütunları Güncelleyen 5 UPDATE İşlemi**

### **a. id'ye Göre name Güncellemesi**
```sql
UPDATE employee
SET name = 'aysu'
WHERE id = 1;
```

### **b. birthday'e Göre email Güncellemesi**
```sql
UPDATE employee
SET email = 'aysukilic99@gmail.com'
WHERE birthday = '2025-01-08';
```

### **c. name'e Göre birthday Güncellemesi**
```sql
UPDATE employee
SET birthday = '2000-01-01'
WHERE name = 'Janeczka';
```

### **d. email'e Göre name Güncellemesi**
```sql
UPDATE employee
SET name = 'Asli'
WHERE email = 'jspeakman12@apache.org';
```

### **e. id Aralığına Göre Toplu name Güncellemesi**
```sql
UPDATE employee
SET name = 'Isimsiz
WHERE id BETWEEN 30 AND 40;
```

---

## **5. Her Sütuna Göre Satır Silecek 5 DELETE İşlemi**

### **a. id'ye Göre Satır Silme**
```sql
DELETE FROM employee
WHERE id = 7;
```

### **b. name'e Göre Satır Silme**
```sql
DELETE FROM employee
WHERE name = 'Ruben';
```

### **c. birthday'e Göre Satır Silme**
```sql
DELETE FROM employee
WHERE birthday = '10/29/2024';
```

### **d. email'e Göre Satır Silme**
```sql
DELETE FROM employee
WHERE email = 'rbateman15@dedecms.com';
```

### **e. id Aralığına Göre Toplu Satır Silme**
```sql
DELETE FROM employee
WHERE id BETWEEN 30 AND 40;
```

---

## **6. Sonuçları Kontrol Etmek İçin**

Tabloyu görüntülemek için:
```sql
SELECT * FROM employee;
```
