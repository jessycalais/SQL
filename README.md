### :dart: Objetivo:
Este repositório possui consultas a dados públicos disponíveis no **BigQuery** a fim de demonstrar minhas habilidades com SQL.

### :pencil: Conteúdo:
**1) Subconsultas na cláusula CASE - com JOIN**  

O arquivo **`sql_subconsultas_case.md`** contém uma consulta com o uso das seguintes ferramentas do **SQL**:
* `SELECT`, `FROM`, `WHERE`, `GROUP BY`, `ORDER BY`;
* `DISTINCT`, `CASE`, `INNER JOIN`;
* `AND`, `BETWEEN`, `COUNT()`, `EXTRACT()`;
* `Subconsultas`.
  
Utilizando esses conceitos foi possível *pivotar* os dados sem utilizar a cláusula `PIVOT`.  
> **NOTA:** Caso queira consultar estes mesmos dados, utilize essas tabelas:
> * `bigquery-public-data.austin_bikeshare.bikeshare_trips`;
> * `bigquery-public-data.austin_bikeshare.bikeshare_stations`.

---

**2) Subconsultas na cláusula CASE - sem JOIN e com LIKE**  

O arquivo **`pivotar_case_sql.md`** contém uma consulta com o uso das seguintes ferramentas do **SQL**:
* `SELECT`, `FROM`, `WHERE`, `GROUP BY`;
* `LIKE`, `CASE`;
* `AND`, `OR`, `ROUND()`, `COUNT()`;
* `Subconsultas`.

Utilizando esses conceitos foi possível *pivotar* os dados sem utilizar a cláusula `PIVOT`.   
Além disso, foi possível verificar a quantidade/porcentagem de vezes que o termo ***education*** foi tratado em algumas matérias da BBC.
> **NOTA:** Caso queira consultar estes mesmos dados, utilize essa tabela:
> * `bigquery-public-data.bbc_news.fulltext`.

---

**3) Funções de Agregação & WHERE com muitas condições**

O arquivo **`funcoes_agregacao_sql.md`** contém uma consulta com o uso das seguintes ferramentas do **SQL**:
* `SELECT`, `FROM`, `WHERE`, `GROUP BY`, `ORDER BY`;
* `DISTINCT`;
* `AND`, `OR`, `ROUND()`;
* `MIN()`, `MAX()`, `AVG()`.

Utilizando esses conceitos foi possível obter algumas informações sobre possíveis mudanças nas notas de Matemática no SAEB antes e depois do ano 2020 (COVID-19) 
> **NOTA:** Caso queira consultar estes mesmos dados, utilize essa tabela:
> * `basedosdados.br_inep_saeb.municipio`.

---

**4) CTE com WITH & funções de agregação**  

O arquivo **`CTE_WITH.md`** contém uma consulta com o uso das seguintes ferramentas do **SQL**:
* `SELECT`, `FROM`, `WHERE`, `GROUP BY`, `ORDER BY DESC`, `LIMIT`;
* `SUM()`;
* `UNION ALL`;
* `Tabelas temporárias - WITH`.
  
Utilizando esses conceitos foi possível determinar os três países com mais casos de COVID-2019 registrados nos anos de 2019 e 2020 (TOP 3).
> **NOTA:** Caso queira consultar estes mesmos dados, utilize essa tabela:
> * `bigquery-public-data.covid19_ecdc.covid_19_geographic_distribution_worldwide`.
