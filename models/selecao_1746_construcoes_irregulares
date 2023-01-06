
SELECT 
id_chamado, data_inicio, data_fim, 
id_logradouro, numero_logradouro, longitude, latitude,
nome_unidade_organizacional, id_unidade_organizacional_mae,
tipo, subtipo, 
status, situacao, tipo_situacao, dentro_prazo,
ST_GEOGPOINT(longitude, latitude) AS geometry 

FROM `datario.administracao_servicos_publicos.chamado_1746`
WHERE subtipo IN (	
  
   'Demolição'
	,'Fiscalização de obras irregulares em comunidade - Áreas de Especial Interesse Social'
	,'Fiscalização de obras em terreno invadido em Áreas de Especial Interesse Social'
	,'Fiscalização de obras em andamento em Áreas Especiais'
	,'Fiscalização de obras em comunidade'
	,'Fiscalização de obras em comunidades'
	,'Fiscalização de obras sem licença de expansão de comunidade'
	
	,'Fiscalização de construção irregular em áreas ambientalmente protegidas'
	,'Fiscalização de ocupação por atividade irregular na natureza'
	
	,'Vistoria em construção irregular'
  ,'Vistoria em invasão'

  )

AND categoria IN ('Serviço')
AND numero_logradouro IS NOT NULL;