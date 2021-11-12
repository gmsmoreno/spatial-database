# COMMAND LINE PROMPT
-- PARA FAZER DIRETO COM O psql DEFINA O ARQUIVO DO EXECUTÁVEL, O SRID, O NOME.SHP DO ARQUIVO E DEPOIS O ESQUEMA (NESSE CASO O Public) .nome_da_tabela

-- BASTA CONCATENAR AGORA COM O psql E DEFINIR O HOST COMO localhost, O BANCO DE DADOS COMO nome_do_bd E O USUÁRIO UTILIZADO (NESSE CASO O postgres): 

## tra_pista_ponto_pouso_l.shp
shp2pgsql.exe -s 4674 -W "LATIN1" tra_pista_ponto_pouso_l.shp Public.tra_pista_ponto_pouso_l | psql -h localhost -d sbde -U postgres

## tra_pista_ponto_pouso_p.shp
shp2pgsql.exe -s 4674 -W "LATIN1" tra_pista_ponto_pouso_p.shp Public.tra_pista_ponto_pouso_p | psql -h localhost -d sbde -U postgres



