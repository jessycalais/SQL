```SQL
-- Objetivo: Identificar se houve mudança nas notas de Matemática no SAEB antes e depois do ano 2020 (COVID-19)

SELECT DISTINCT
  ano,
  rede,  
  MIN(media) AS min_matematica,             -- Retorna a nota mínima em matemática no SAEB por rede
  MAX(media) AS max_matematica,             -- Retorna a nota máxima de matemática no SAEB por rede
  ROUND(AVG(media), 2) AS media_matematica  -- Retorna a média das notas de matemática no SAEB por rede
FROM 
  `basedosdados.br_inep_saeb.municipio`
WHERE
  (ano = 2019 OR ano = 2021) 
  AND disciplina = 'MT' 
  AND sigla_uf = 'SP'
  AND (rede = 'Estadual' OR rede = 'Municipal')
GROUP BY
  ano,
  rede
ORDER BY
  ano,
  rede
```
