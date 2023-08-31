# Proposta de Pipeline de ETL para o Bootcamp da Santander 

O objetivo inicial desse projeto é desenvolver um processo de ETL para aplicar os conhecimentos desenvolvidos nos módulos
iniciais. Porem, esse repositório também cumprirá o papel de construir um índice de deflacionamento mensal ao longo dos anos,
para a correção de valores com base no IPCA.

## 1. Extract

Extrair os dados mensais de IPCA por meio da API do IBGE

## 2. Transform

2.1. Transformar os dados Json em DataFrame Pandas.
2.2. Acrescentar uma coluna de Data com base na coluna de valores Ano/Mes
2.3. Manter apenas as colunas Data e IPCA no DataFrame
2.4. Explorar se há existência de inconsistência nos dados (Ex: se há dados NA)
2.5. Cassificar o DataFrame como base na Data, do Data mais recente a mais antiga.
2.6. Acrescentar uma coluna de índice de preços, fixando o valor presente em 1.
2.7. Acrescentat uma coluna de índice de deflacionamento, a partir da coluna de índice de preços.

## 3. Load
Exportar o DataFrame da maneira que preferir. (Ex: Excel)



Link para um artigo sobre a fórmula do Índice de Deflacionamento: <https://downloads.fipe.org.br/publicacoes/bif/bif478-18-24.pdf>
