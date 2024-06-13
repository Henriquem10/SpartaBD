# Codigo para o Case Técnico Sparta - Desenvolvedor Python

O codigo foi feito usando apenas o Jupyter Notebook com a biblioteca do Pandas e Sqlite3. Para rodar o código é apenas necessário rodar as células em ordem.

Os dados foram extraidos do link https://dados.gov.br/dados/conjuntos-dados/cias-abertas-informao-cadastral em formato de csv, e depois pelo python eles foram usados para criar um banco de dados com as informações dos campos CNPJ_CIA, DENOM_SOCIAL e SIT em uma tabela com o nome de cias.

Como o usuário pode querer checar uma data para ver se os campos DENOM_SOCIAL e SIT caso tenham sido alterados foi criado uma segunda tabela chamada changelog em que toda vez que a tabela cias é atualizada ou iniserida com um novos valores é acionado um trigger que pega esses dados e salva na tabela changelog junto com a data de quando a ação foi executada no formato YYYY-MM-DD.
Para realizar as consultas utilizando a data é preciso usar o formato YYYY-MM-DD, sempre fornecendo a data completa.
