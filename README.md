

# All For One - Querys MySQL

## Sobre
 O All For One é um projeto focado em Querys para banco de dados SQL (MySQL). Desde Querys simples até a INNER JOINS avançados.

## Arquivos
Os seguintes arquivos foram desenvolvidos por mim:
- todos os arquivos desafioXX.sql ( do desafio1.sql até o desafio27.sql)
A Trybe forneceu a configuração inicial do projeto no arquivo `package.json`.

## Tecnologias
As seguintes tecnologias foram aplicadas por mim neste projeto:
- Docker;
- Querys MySQL;


## Como executar a aplicação em sua máquina

1. Clone o repositório.
2. Instale as dependências do projeto com o comando `npm install`
3. Se já tiver o MySQL em seu computador, você pode usar o MySQL Workbench e subir o script do banco de dados através do arquivo northwind.sql ou subir um banco de dados docker com o comando `docker-compose up -d`.
4. Segue abaixo os desafios de consulta realizados neste banco de dados. A resolução do Desafio 1 está no arquivo desafio1.sql, a resolução do desafio 2 no arquivo desafio2.sql, assim sucessivamente.

## Desafios
## Desafios Iniciais

1 - Exiba apenas os nomes dos produtos na tabela products.

2 - Exiba os dados de todas as colunas da tabela products.

3 - Escreva uma query que exiba os valores da coluna que representa a primary key da tabela products.

4 - Conte quantos registros existem na coluna product_name da tabela products.

5 - Monte uma query que exiba os dados da tabela products a partir do quarto registro até o décimo terceiro.

6 - Exiba os dados das colunas product_name e id da tabela products de maneira que os resultados estejam em ordem alfabética dos nomes.

7 - Mostre apenas os ids dos 5 últimos registros da tabela products (a ordernação deve ser baseada na coluna id).

8 - Faça uma consulta que retorne três colunas, respectivamente, com os nomes 'A', 'Trybe' e 'eh', e com valores referentes a soma de '5 + 6', a string 'de', a soma de '2 + 8'.

## Desafios sobre filtragem de dados

9 - Mostre todos os valores de notes da tabela purchase_orders que não são nulos.

10 - Mostre todos os dados da tabela purchase_orders em ordem decrescente, ordenados por created_by em que o created_by é maior ou igual a 3.

    Ordene também os resultados pelo id de forma crescente, como critério de desempate para a ordenação.

11 - Exiba os dados da coluna notes da tabela purchase_orders em que seu valor de Purchase generated based on Order é maior ou igual a 30 e menor ou igual a 39.


12 - Mostre as submitted_date de purchase_orders em que a submitted_date é do dia 26 de abril de 2006.

13 - Mostre o supplier_id das purchase_orders em que o supplier_id seja 1 ou 3.

14 - Mostre os resultados da coluna supplier_id da tabela purchase_orders em que o supplier_id seja maior ou igual a 1 e menor ou igual 3.

15 - Mostre somente as horas (sem os minutos e os segundos) da coluna submitted_date de todos registros da tabela purchase_orders.

    No resultado, a hora extraída da coluna submitted_date deve ser chamada de submitted_hour.

16 - Exiba a submitted_date das purchase_orders que estão entre 2006-01-26 00:00:00 e 2006-03-31 23:59:59.

17 - Mostre os registros das colunas id e supplier_id das purchase_orders em que os supplier_id sejam tanto 1, ou 3, ou 5, ou 7.

18 - Mostre todos os registros de purchase_orders que tem o supplier_id igual a 3 e status_id igual a 2.

19 - Mostre a quantidade de pedidos que foram feitos na tabela orders pelo employee_id igual a 5 ou 6, e que foram enviados através do método(coluna) shipper_id igual a 2.

    No resultado, a coluna que contém a contagem de pedidos deve ser chamada de orders_count.

## Desafios de manipulação de tabelas

20 - Adicione à tabela order_details um registro com order_id: 69, product_id: 80, quantity: 15.0000, unit_price: 15.0000, discount: 0, status_id: 2, date_allocated: NULL, purchase_order_id: NULL e inventory_id: 129.

21 - Adicione com um único INSERT, duas linhas à tabela order_details com os mesmos dados do requisito 20.

22 - Atualize os dados de discount do order_details para 15.

warning Para testar localmente, pode ser necessário utilização do SAFE UPDATE, porém não é necessário adicionar a instrução do SAFE UPDATE no arquivo desafio22.sql junto a query, pois o próprio avaliador irá ajustar isso.

23 - Atualize os dados da coluna discount da tabela order_details para 30, onde o valor na coluna unit_price seja menor que 10.0000.

24 - Atualize os dados da coluna discount da tabela order_details para 45, onde o valor na coluna unit_price seja maior que 10.0000 e o id seja um número entre 30 e 40.

25 - Delete todos os dados em que a unit_price da tabela order_details seja menor que 10.0000.

26 - Delete todos os dados em que a unit_price da tabela order_details seja maior que 10.0000.

27 - Delete todos os dados da tabela order_details.
