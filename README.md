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
Rosalia_TP> load data local infile "c:/Users/USER/Desktop/Mi_Proyecto/sesion03/
            Mis_Datos/cwurData.csv" into table ranking fields terminated by ","
            ;
(1148, 'The used command is not allowed with this MariaDB version')
Rosalia_TP> load data local infile "c:Users/USER/Desktop/Mi_Proyecto/sesion03/M
            is_Datos/cwurData.csv" into table ranking fields terminated by ",";

(1148, 'The used command is not allowed with this MariaDB version')
Rosalia_TP> load data local infile "C: Users/USER/Desktop/Mi_Proyecto/sesion03/
            Mis_Datos/cwurData.csv" into table ranking fields terminated by ","
            ;
(1148, 'The used command is not allowed with this MariaDB version')
Rosalia_TP> load data local infile "C:\Users\USER\Desktop\Mi_Proyecto\sesion03\
            Mis_Datos\cwurData.csv" into table ranking fields terminated by ","
            ;
(1148, 'The used command is not allowed with this MariaDB version')
Rosalia_TP> load data local infile "C:\Users\USER\Desktop\Mi_Proyecto\sesion03\
            Mis_Datos\cwurData.csv" into table ranking fields terminated by ","
            ;
(1148, 'The used command is not allowed with this MariaDB version')
Rosalia_TP> load data local infile "C:/Users/USER/Desktop/Mi_Proyecto/sesion03/
            Mis_Datos/cwurData.csv" into table ranking fields terminated by ","
            ;
(1148, 'The used command is not allowed with this MariaDB version')
Rosalia_TP>
