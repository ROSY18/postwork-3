# postwork-3



EN LA CONSOLA DE GIT BASH 

  478  cd desktop
  479  pwd
  480  cd desktop
  481  cd Mi_Proyecto
  482  ls
  483  mkdir sesion03
  484  ls
  485  cp -a ../../ Mis_Datos/sesion03/Datos .
  486  cp -a ../../ Mis_Datos/sesion03/Datos
  487  cp -a ../../ sesion03/Mis_Datos
  488  cp -a ../../ sesion03/Mis_Datos .
  489  ls
  490  ls
  491  cd sesion03
  492  ls
  493  cd ..
  494  cp Mis_Datos sesion03
  495  cp  -r Mis_Datos sesion03
  496  cd sesion03
  497  ls


EN LA TEMINAL DE MINICONDA

(none)> show databases;
+--------------------+
| Database           |
+--------------------+
| ANDREA             |
| Adrii_Merlin       |
| FranciscoGarcia_DB |
| Jazmin             |
| Lilia              |
| ROSS               |
| Rosalia            |
| Rosalia_TP         |
| Sam                |
| Sergio             |
| Zamby              |
| information_schema |
| janet              |
| maria              |
| mysql              |
| performance_schema |
+--------------------+

16 rows in set
Time: 0.169s
(none)> use Rosalia_TP;
You are now connected to database "Rosalia_TP" as user "root"
Time: 0.083s
Rosalia_TP> create table ranking(
            world_rank int primary key,
            institution varchar (30),
            country varchar (20),
            national_rank int,
            quality_of_education int,
            alumni_employment int,
            quality_of_faculty int,
            publications int,
            influence int,
            citations int,
            broad_impact int,
            patents int,
            score int,
            year_ int);
Query OK, 0 rows affected
Time: 0.155s
Rosalia_TP> show tables;
+----------------------+
| Tables_in_Rosalia_TP |
+----------------------+
| VANILLA_TP           |
| ranking              |
+----------------------+
Rosalia_TP> show tables;
+----------------------+
| Tables_in_Rosalia_TP |
+----------------------+
| VANILLA_TP           |
| ranking              |
+----------------------+
2 rows in set
Time: 0.174s



Rosalia_TP> load data local infile "C:/Users/USER/Desktop/Mi_Proyecto/sesion03/
            Mis_Datos/cwurData.csv" into table ranking fields terminated by ","
            ;
Query OK, 1001 rows affected
Time: 2.743s
Rosalia_TP> select
(1064, "You have an error in your SQL syntax; check the manual that corresponds
to your MariaDB server version for the right syntax to use near '' at line 1")
Rosalia_TP> select *from ranking;
+------------+--------------------------------+----------------------+----------
-----+----------------------+-------------------+--------------------+----------
----+-----------+-----------+--------------+---------+-------+-------+
| world_rank | institution                    | country              | national_
rank | quality_of_education | alumni_employment | quality_of_faculty | publicati
ons | influence | citations | broad_impact | patents | score | year_ |
+------------+--------------------------------+----------------------+----------
-----+----------------------+-------------------+--------------------+----------
----+-----------+-----------+--------------+---------+-------+-------+
| 0          | institution                    | country              | 0
     | 0                    | 0                 | 0                  | 0
    | 0         | 0         | 0            | 0       | 0     | 0     |
| 1          | "Harvard University"           | USA                  | 1
     | 7                    | 9                 | 1                  | 1
    | 1         | 1         | 0            | 5       | 100   | 2012  |
| 2          | "Massachusetts Institute of Te | USA                  | 2
     | 9                    | 17                | 3                  | 12
    | 4         | 4         | 0            | 1       | 92    | 2012  |
| 3          | "Stanford University"          | USA                  | 3
     | 17                   | 11                | 5                  | 4
    | 2         | 2         | 0            | 15      | 90    | 2012  |
| 4          | "University of Cambridge"      | United Kingdom       | 1
     | 10                   | 24                | 4                  | 16
    | 16        | 11        | 0            | 50      | 86    | 2012  |
| 5          | "California Institute of Techn | USA                  | 4
     | 2                    | 29                | 7                  | 37
    | 22        | 22        | 0            | 18      | 85    | 2012  |
| 6          | "Princeton University"         | USA                  | 5
     | 8                    | 14                | 2                  | 53
    | 33        | 26        | 0            | 101     | 83    | 2012  |
| 7          | "University of Oxford"         | United Kingdom       | 2
     | 13                   | 28                | 9                  | 15
    | 13        | 19        | 0            | 26      | 82    | 2012  |
| 8          | "Yale University"              | USA                  | 6
-- Más  --
