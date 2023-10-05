# SQL-DADOS
Tratamento de Dados utilizando SQL

Esses dados foram extraidos do Kaggle, uma plataforma usada para treino, desafios e com muitas bases de dados. Estou utilizando o SQLITE online para tratamente desses dados. Vamos descobrir alguns dados e trata-los.

-Primeiro descobri a média de preço de todos os produtos, com marca, tipo, armazenamento. Porém, estes dados estavam em rupias indianas, então fiz a conversão deles.
-Depois de convertidos, crie uma view para melhorar a análise. Ordenei por media de preço desc.

-Durante a tratativa desses dados, notei que Lenovo aparecia como 'lenovo' e 'Lenovo', fazendo com que o preço médio estivesse errado, pois 'lenovo' tinha um ticket médio muito maior que 'Lenovo'.

-Após isso crei uma case, que caso fosse 'lenovo', retornaria como 'Lenovo' caso nenhum dos dois, retornaria como brand (marca). E agrupei por CASE.

-Depois do comando case, observamos que o ticket médio de 'Lenovo' era na verdade 45136. Isso pode ocorrer quando o sistema é case-sensitive, por isso tomamos cuidado em relação a isso.

-Foi pedido também que descobrissemos os impactos da memória de nas vendas. Podemos perceber que temos nomes diferentes, mas são da mesma categoria.
Então para tratar esses dados novamente usei o comando CASE e ordenei pelo maior ticket. Percebemos que DDR3 tem um ticker maior que DDR4, que para os padrões da tecnologia de hoje, é incomum, isso poderia abrir uma brecha para novas análises.

-No final, somamos tudo e analisamos que mesmo tendo uma média de preço menor, as vendas do DDR4 são esmagadoras em comparação com as outras.

Insights relevantes: 

Lenovo na verdade tinha um ticket médio muito abaixo do relatado.

DDR4 com um ticket médio menor, tem muito mais impacto que as outras memórias em relação as vendas.

Sobre o caso do DDR3, pode haver marcas elevando consideravelmente o preço das memórias, visto que ela vem agrupada em computadoras das marcas, como a Apple.

![Port1](https://github.com/JulioA/SQL-DADOS/assets/146854621/3d3e0d23-346e-4a22-8b1d-c8036a7b4c2c)
![Port2](https://github.com/JulioA/SQL-DADOS/assets/146854621/67f108a9-6e18-41cc-aa24-6d2e7d1cf7d5)
![Port3](https://github.com/JulioA/SQL-DADOS/assets/146854621/4b895f7f-24be-4004-b8b7-f4333124cd1a)
![Port4](https://github.com/JulioA/SQL-DADOS/assets/146854621/93f9d9ff-adb8-4516-bb02-4418f6281551)
![Port5](https://github.com/JulioA/SQL-DADOS/assets/146854621/4aac9670-7bb6-421c-9ae3-b0f8d44aa2fc)
![Port6](https://github.com/JulioA/SQL-DADOS/assets/146854621/54c85aad-2dd9-4a19-9193-4feedd6c870d)
![Port7](https://github.com/JulioA/SQL-DADOS/assets/146854621/bdd0a85a-2774-4c13-8407-eaeb7d1d1dd7)
![Port8](https://github.com/JulioA/SQL-DADOS/assets/146854621/69e56944-b295-4990-a37a-518682fbde12)
![port9](https://github.com/JulioA/SQL-DADOS/assets/146854621/33532955-d493-44ce-b8c1-fce4dca17d1d)
![Port10](https://github.com/JulioA/SQL-DADOS/assets/146854621/a6e7bdc2-01d6-4103-a3f1-167ed1524d8e)
![Port11](https://github.com/JulioA/SQL-DADOS/assets/146854621/8670aab4-ae48-484a-b8c9-a0c010da1eb1)
