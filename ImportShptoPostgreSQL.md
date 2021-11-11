## COMMAND LINE PROMPT
-- PARA FAZER DIRETO COM O psql DEFINA O ARQUIVO DO EXECUTÁVEL, O SRID, O NOME.SHP DO ARQUIVO E DEPOIS O ESQUEMA (NESSE CASO O Public) .nome_da_tabela

-- BASTA CONCATENAR AGORA COM O psql E DEFINIR O HOST COMO localhost, O BANCO DE DADOS COMO nome_do_bd E O USUÁRIO UTILIZADO (NESSE CASO O postgres): 

temp>shp2pgsql.exe -s 4674 tis_sirgas2000.shp Public.tis_sirgas2000 | psql -h localhost -d sbde -U postgres

