
# introdução 

Fomos contratado pela area de marketing de um banco de NYC para analisar os dados e dividir os clientes em  grupos com caracteristicas semelhantes, com intuito de criar campanhas que melhor se adeque a cada tipo de grupo de cliente, os dados analisados estão disponivel no <a href="https://www.kaggle.com/datasets/arjunbhasin2013/ccdata">Kaggle</a> , para esse projeto usaramos tecnicas para separar os clientes em clusters.

### Contexto do negócio

No banco à diversos comportamentos que podemos identificar dos clientes através de suas movimentações em sua conta e a contração de produtos, tem clientes que pagam suas vendas a vista, há clientes que pagam o mínimo da fatura, nosso objetivo será identificar esses padrões e agrupar os clientes na caracteristica que melhor se adeque ao seu perfil.

### Dados

Os dados como foram extraidos da plataforma kaggle

Abaixo os atributos:

<table>

  
  <tr><td><b><i>Atributo</b><i></td><td><b><i>Descrição</b></i></td></tr>  

  <tr><td><b>CUSTID</b></td><td>Identificação do cliente</td></tr>
  <tr><td><b>BALANCE</b></td><td>Saldo para fazer compras</td></tr>
  <tr><td><b>BALANCEFREQUENCY</b></td><td>Frequencia que o saldo é atualizado (1 = frequente, 0 = não frequente)</td></tr>
  <tr><td><b>PURCHASES</b></td><td>Quantidade de compras realizadas</td></tr>
  <tr><td><b>ONEOFFPURCHASES</b></td><td>Quantidade de compras feitas "de uma só vez"</td></tr>
  <tr><td><b>INSTALLMENTSPURCHASES</b></td><td>Quantidade de compras parceladas</td></tr>
  <tr><td><b>CASHADVANCE</b></td><td>Dinheiro adinhantado</td></tr>
  <tr><td><b>PURCHASESFREQUENCY</b></td><td>Com que frequência as compras estão sendo feitas, pontuação entre 0 e 1 (1 = comprado com frequência, 0 = não comprado com frequência)</td></tr>
  <tr><td><b>ONEOFFPURCHASESFREQUENCY</b></td><td>Frequencia de compras a vista (1 = frequente, 0 = não frequente)</td></tr>
  <tr><td><b>PURCHASESINSTALLMENTSFREQUENCY</b></td><td> Frequencia de compras parceladas ( 1 = frequente, 0 = não frequente)</td></tr>
  <tr><td><b>CASHADVANCEFREQUENCY</b></td><td>Frequencia de saques de dinheiro adiantado</td></tr>
  <tr><td><b>CASHADVANCETRX</b></td><td>Número de transações feitas com "Cash in Advanced"</td></tr>
  <tr><td><b>PURCHASESTRX</b></td><td>Número de compras</td></tr>
  <tr><td><b>CREDITLIMIT</b></td><td>Limite de cartão de crédito</td></tr>
  <tr><td><b>PAYMENTS</b></td><td>Valor Pago</td></tr>
  <tr><td><b>MINIMUM_PAYMENTS</b></td><td>Valor mínimo pago</td></tr>
  <tr><td><b>PRCFULLPAYMENT</b></td><td>Percentual de pagamento de fatura "completa"</td></tr>
  <tr><td><b>TENURE</b></td><td>Posse do titular do cartão</td></tr>

</table> 
 

### Analise Exploratoria
  
<ol>
  <li>Valores 'NaN'</li>
  <li>Verificação do tipo de dados</li>
  <li>Estatistica descritiva</li>
</ol>

### Preparação dos dados
  
Apos realizar analise descritiva dos dados, vamos realizar a preparação dos dados.
  
### KMEANS
Nessa etapa com os dados pré processados, vamos utilizar o Kmeans para realizar o agrupamento dos dados, vamos realizar com 20 clusters e validar com quantos clusters nós temos menos erro.
<br>
 Apos os teste, vamos usar 8 clusters para nossa base pois é o número de cluster onde nosso teste teve menos erro.
  
 ### Conclusão

 Apos o Agrupamento dos clientes em clusters tivemos os seguintes insights para os clientes e baseado nessas informações podemos repassar ao time de marketing realizar as campanhas.
  
<n>Grupo 0 (VIP/Prime)</n>: limite do cartão alto (15570) e o mais alto percentual de pagamento da fatura completa (0.47). Aumentar o limite do cartão e o hábito de compras

<n>Grupo 3</n>: Clientes que pagam poucos juros para o banco e são cuidadosos com seu dinheiro. Possui menos dinheiro na conta corrente (104) e não sacam muito dinheiro do limite do cartão (302). 23% de pagamento da fatura completa do cartão de crédito

<n>Grupo 5</n>: usam o cartão de crédito como "empréstimo" (setor mais lucrativo para o banco), possuem muito dinheiro na conta corrente (5119) e sacam muito dinheiro do cartão de crédito (5246), compram pouco (0.3) e usam bastante o limite do cartão para saques (0.51). Pagam muito pouco a fatura completa (0.03)

<n>Grupo 7 (clientes novos)</n>: clientes mais novos (7.23) e que mantém pouco dinheiro na conta corrente (863)
 

  
  

