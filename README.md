### :dart: Objetivo:
Este repositório possui consultas a dados públicos disponíveis no **BigQuery** a fim de demonstrar minhas habilidades com SQL.

### :pencil: Conteúdo:
**1) Subconsultas na cláusula CASE - com JOIN**  

O arquivo **`sql_subconsultas_case.md`** contém uma consulta com o uso das seguintes ferramentas do **SQL**:
* `SELECT`, `FROM`, `WHERE`, `GROUP BY`, `ORDER BY`;
*  `COUNT()`, `DISTINCT`, `CASE`, `INNER JOIN`;
* `AND`, `EXTRACT()`, `BETWEEN`;
* `Subconsultas`.
  
Utilizando esses conceitos foi possível *pivotar* os dados sem utilizar a cláusula `PIVOT`.  
> **NOTA:** Caso queira consultar estes mesmos dados, utilize essas tabelas:
> * `bigquery-public-data.austin_bikeshare.bikeshare_trips`;
> * `bigquery-public-data.austin_bikeshare.bikeshare_stations`.

---

**2) Subconsultas na cláusula CASE - sem JOIN e com LIKE**  

O arquivo **`pivotar_case_sql.md`** contém uma consulta com o uso das seguintes ferramentas do **SQL**:
* `SELECT`, `FROM`, `WHERE`, `GROUP BY`;
*  `COUNT()`, `LIKE`, `CASE`;
* `AND`, `OR`, `ROUND()`;
* `Subconsultas`.

Utilizando esses conceitos foi possível *pivotar* os dados sem utilizar a cláusula `PIVOT`.  
> **NOTA:** Caso queira consultar estes mesmos dados, utilize essa tabela:
> * `bigquery-public-data.bbc_news.fulltext`.

---

**3) Funções de Agregação & WHERE com muitas condições**

O arquivo **`funcoes_agregacao_sql.md`** contém uma consulta com o uso das seguintes ferramentas do **SQL**:
* `SELECT`, `FROM`, `WHERE`, `GROUP BY`, `ORDER BY`;
* `DISTINCT`, `AND`, `OR`, `ROUND()`;
* `MIN()`, `MAX()`, `AVG()`.

Utilizando esses conceitos foi possível obter algumas informações sobre possíveis mudanças nas notas de Matemática no SAEB antes e depois do ano 2020 (COVID-19) 
> **NOTA:** Caso queira consultar estes mesmos dados, utilize essa tabela:
> * `basedosdados.br_inep_saeb.municipio`.
