# Telecom-X-Análise-de-Evasão-de-Clientes
## Autor: Vicente V Pascoal

## Introdução: 
O principal objetivo da nossa analise é **determinar** possíveis motivos para os clientes do Telecom acabarem **saindo** do nosso serviço. Uma das suposições é aqueles clientes que contratam nossos serviços por tempos reduzidos, ou seja, contratam a gente apenas por alguns meses e não fecham um contrato mais longo. Já a segunda vimos que os clientes que pagam o seviço usando check eletronico acabam saindo mais dos nossos serviços.  

## Limpeza e Tratamento de Dados:
Comecei carregando o arquivo dentro do collab em vez de criar uma variável com a url do dataset, pois acho mais prático, após isso atribui os dados a uma variável.
Comecei análisando o dataset e percebi que todas as informações estavam com o tipo object, já que a grande marioria possuia um dicionário dentro delas dificultando um pouco nossa análise. 
Verifiquei se havia algum dado repetido e aparentemente não havia, mas após tentar verificar cada dicionário foi percebido que havia sim algumas linhas repetidas e a melhor decisão foi exclui-las. (Depois percebi que tinham linhas inconsistentes, já que na coluna os únicos valores que poderiam existir é "Yes" e "No", mas no final das contas existiam strings vazias que foram excluídas posteriormente).
Em penúltimo criei uma coluna pra entendermos o gasto diário do cliente usando os dados de gasto mensal do cliente.
Por último padronizei os valores que tinham valor de "Yes" e "No" para 1 ou 0 (Menos na coluna Churn)

## Análise Exploratória de Dados:
Foram realizadas 5 análises, sendo elas: 
 - Verificação de média, mediana e desvio padrão
 - Quantidade de Evasão através de um gráfico de pizza
 - Relação entre o gênero e a quantidade de evasão utilizando gráfico de barras 
 - Relação entre o tipo do contrato e a quantidade de evasão utilizando gráfico de barras
 - Relação entre o método de pagamento e a quantidade de evasão utilizando gráfico de barras  

## Conclusões e Insights:
Após a análise dos gráficos realizados chegamos a conclusão que os clientes que utilizam método de pagamento que não é automático acaba cancelando mais o nosso serviço, um outro ponto também são os clientes que contratam nosso serviço por um período curto de tempo. 

## Recomendações:
Portanto algumas possíveis ideias para resolvermos esse problema seria ou adicionarmos algum tipo de recompensa para pessoas que utilizam métodos de pagamentos automáticos, impulsionando pessoas a migrarem. Outra ideia seria talvez retirar outros métodos de pagamentos, mas isso nos faria perder alguns clientes. 
Já na parte do tipo do contrato poderemos dar algum tipo de desconto pra pessoa contratar nosso serviço anual ou por 2 anos. 
