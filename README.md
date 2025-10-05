Este projeto contém o script SQL para a criação e configuração de um banco de dados relacional (SQL Server) focado em dados de Produto Interno Bruto (PIB) de municípios do estado de São Paulo.
O esquema de banco de dados foi projetado para:

- Integridade de dados: As tabelas MUNICIPIO, PIB, e PIB_SETOR são conectadas por chaves primárias e estrangeiras, garantindo a integridade referencial dos dados.

- Automação e Consistência: Triggers foram implementadas para automatizar a atualização do PIB total com base nos valores por setor, assegurando a consistência das informações.

- Auditoria de Alterações: Uma tabela de auditoria dedicada (Auditoria) é utilizada para registrar todas as operações de INSERT, UPDATE e DELETE nas tabelas principais. As triggers de auditoria capturam detalhes como o tipo de operação, o usuário, a data/hora, e os dados antigos e novos em formato JSON, proporcionando um histórico completo e rastreável.

Este projeto pode servir como uma base sólida para análises econômicas, dashboards de visualização de dados e aplicações que necessitem de um modelo robusto para gerenciar dados de PIB municipal.
