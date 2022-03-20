
## Exercício 2

```
CREATE TABLE login ( 
    id int NOT NULL, 
    email varchar(100) NOT NULL, 
    status varchar(10) NOT NULL, 
    last_access date DEFAULT NULL,
    token varchar(255),
    PRIMARY KEY (id)
);
```

Aqui foi necessário um pequeno ajuste, visto que as aspas(plicas) na primary key estavam a dar erro.
Bastou sua remoção e já tive sucesso na execução.

## Exercício 4

```
SELECT * FROM LOGIN WHERE ID = 1;

SELECT * FROM LOGIN WHERE STATUS = 'ATIVO' AND STATUS = 'INATIVO';

SELECT * FROM LOGIN WHERE STATUS = 'ATIVO' OR STATUS = 'INATIVO';

SELECT * FROM LOGIN WHERE TOKEN = NULL;

SELECT * FROM LOGIN WHERE STATUS = 'ATIVO' AND TOKEN IS NOT NULL;

```

Aqui, uma pequena correção na última query, onde o filtro não funcionou como esperado. Neste caso, o ajuste foi para IS NOT NULL e tudo correu bem.