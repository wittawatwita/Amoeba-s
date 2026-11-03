mysql -u root -p #เพื่อเข้า SQL
Enter password: #enter ถ้าไม่มีรหัส

show database; #แสดงทั้งหมดของ database
MariaDB [(none)]> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| cal                |
| calculator         |
| calculator_history |
| catone             |
| information_schema |
| koidgay            |
| mysql              |
| performance_schema |
| phpmyadmin         |
| tankongay          |
| test               |
| today              |
| x.com              |
+--------------------+
13 rows in set (0.053 sec)


USE phpmyadmin; #เพื่อเข้าไปในแต่ละฟิว
MariaDB [(none)]> USE phpmyadmin;
Database changed
MariaDB [phpmyadmin]>


Exit; หรือ ctel + c #เพื่อออกทั้งหมด


show tables; #เพื่อโชว์แต่ละอันที่อยู่ในฟิว
MariaDB [phpmyadmin]> show tables;
+------------------------+
| Tables_in_phpmyadmin   |
+------------------------+
| pma__bookmark          |
| pma__central_columns   |
| pma__column_info       |
| pma__designer_settings |
| pma__export_templates  |
| pma__favorite          |
| pma__history           |
| pma__navigationhiding  |
| pma__pdf_pages         |
| pma__recent            |
| pma__relation          |
| pma__savedsearches     |
| pma__table_coords      |
| pma__table_info        |
| pma__table_uiprefs     |
| pma__tracking          |
| pma__userconfig        |
| pma__usergroups        |
| pma__users             |
+------------------------+
19 rows in set (0.004 sec)


DESCRIBE pma__bookmark; #เพื่อเข้าไปดูรายละเอียดอีกที
MariaDB [phpmyadmin]> DESCRIBE pma__bookmark;
+-------+------------------+------+-----+---------+----------------+
| Field | Type             | Null | Key | Default | Extra          |
+-------+------------------+------+-----+---------+----------------+
| id    | int(10) unsigned | NO   | PRI | NULL    | auto_increment |
| dbase | varchar(255)     | NO   |     |         |                |
| user  | varchar(255)     | NO   |     |         |                |
| label | varchar(255)     | NO   |     |         |                |
| query | text             | NO   |     | NULL    |                |
+-------+------------------+------+-----+---------+----------------+
5 rows in set (0.015 sec)
