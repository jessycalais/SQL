```SQL
-- Objetivo: Determinar os três países com mais casos de covid registrados nos anos de 2019 e 2020 (TOP 3)
-- Dados utilizados: dados públicos disponíveis no BigQuery

WITH
  year_2019 AS (
    SELECT
        year, 
        countries_and_territories, 
        SUM(daily_confirmed_cases) AS total_cases
    FROM
        `bigquery-public-data.covid19_ecdc.covid_19_geographic_distribution_worldwide`
    WHERE 
        year = 2019
    GROUP BY
        year, 
        countries_and_territories 
    ORDER BY
        total_cases DESC
    LIMIT 3),

  year_2020 AS (
    SELECT
        year, 
        countries_and_territories, 
        SUM(daily_confirmed_cases) AS total_cases
    FROM
        `bigquery-public-data.covid19_ecdc.covid_19_geographic_distribution_worldwide`
    WHERE
        year = 2020
    GROUP BY
        year,
        countries_and_territories
    ORDER BY
        total_cases DESC
    LIMIT 3)

SELECT
  year_2019.year, year_2019.countries_and_territories, year_2019.total_cases  
FROM
  year_2019

UNION ALL

SELECT
  year_2020.year, year_2020.countries_and_territories, year_2020.total_cases
FROM
  year_2020
```
