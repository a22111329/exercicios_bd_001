## Exercício 1
1.1
```
CREATE TABLE login ( 
    id int NOT NULL, 
    email varchar(100) NOT NULL, 
    status varchar(10) NOT NULL, 
    last_access date DEFAULT NULL,
    token varchar(255),
    PRIMARY KEY ('id')
);
```

1.2 

LOGIN(**id**, email, status, last_access, token)

## Exercício 2

```
CREATE TABLE login ( 
    id int NOT NULL, 
    email varchar(100) NOT NULL, 
    status varchar(10) NOT NULL, 
    last_access date DEFAULT NULL,
    token varchar(255),
    PRIMARY KEY ('id')
);
```


## Exercício 3

1.


| id | email           | status  | last_access | token                 |
|----|-----------------|---------|-------------|-----------------------|
| 1  | alfa@gmail.com  | ATIVO   | 2022/03/14  | asdfaAxvdxfvx9809dsf9 |
| 2  | beta@gmail.com  | INATIVO | 2021/04/12  | 809d8sfsdafDdcxv00989 |
| 3  | gama@gmail.com  | ATIVO   | 2020/10/05  | afasdf9a8sdfa8d90sf8a |
| 4  | theta@gmail.com | ATIVO   | 2022/03/14  | opiiopiop90afadsAaacC |
| 5  | omega@gmail.com | INATIVO | 2019/11/11  | 6878667HJKHJKHJK99dsf |

2.

```
INSERT INTO LOGIN VALUES(1, 'alfa@gmail.com', 'ATIVO', '2022/03/14', 'asdfaAxvdxfvx9809dsf9');
INSERT INTO LOGIN VALUES(2, 'beta@gmail.com', 'INATIVO', '2021/04/12', '809d8sfsdafDdcxv00989');
INSERT INTO LOGIN VALUES(3, 'gama@gmail.com', 'ATIVO', '2020/10/05', 'afasdf9a8sdfa8d90sf8a');
INSERT INTO LOGIN VALUES(4, 'theta@gmail.com', 'ATIVO', '2022/03/14', 'opiiopiop90afadsAaacC');
INSERT INTO LOGIN VALUES(5, 'omega@gmail.com', 'INATIVO', '2019/11/11', '6878667HJKHJKHJK99dsf');
```

## Exercício 4

```
SELECT * FROM LOGIN WHERE ID = 1;

SELECT * FROM LOGIN WHERE STATUS = 'ATIVO' AND STATUS = 'INATIVO';

SELECT * FROM LOGIN WHERE STATUS = 'ATIVO' OR STATUS = 'INATIVO';

SELECT * FROM LOGIN WHERE TOKEN = NULL;

SELECT * FROM LOGIN WHERE STATUS = 'ATIVO' AND TOKEN != NULL;

```


## Exercício 5
1.
```
UPDATE LOGIN SET STATUS = 'ATIVO' WHERE ID = 2;

UPDATE LOGIN SET EMAIL = 'delta@outlook.com' WHERE ID = 1;

UPDATE LOGIN SET TOKEN = '3218181FHKJSDHFasdf' WHERE ID = 3;

```

2.
```
SELECT STATUS FROM LOGIN WHERE ID = 2;

SELECT EMAIL FROM LOGIN WHERE ID = 1;

SELECT TOKEN FROM LOGIN WHERE ID = 3;

```