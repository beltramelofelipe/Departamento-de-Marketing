
# introdução 

Fomos contratado pela area de marketing de um banco de NYC para analisar os dados e dividir os clientes em  grupos com caracteristicas semelhantes, com intuito de criar campanhas que melhor se adeque a cada tipo de grupo de cliente, os dados analisados estão disponivel no <a href="https://www.kaggle.com/datasets/arjunbhasin2013/ccdata">Kaggle</a> , para esse projeto usaramos tecnicas para separar os clientes em clusters.

### Contexto do negócio

No banco à diversos comportamentos que podemos identificar dos clientes através de suas movimentações em sua conta e a contração de produtos, tem clientes que pagam suas vendas a vista, há clientes que pagam o mínimo da fatura, nosso objetivo será identificar esses padrões e agrupar os clientes na caracteristica que melhor se adeque ao seu perfil.

### Dados

Os dados como foram extraidos da plataforma kaggle
<table>
abaixo os atributos:
  <tr><td><b><i>Atributo</b><i></td><td><b><i>Descrição</b></i></td></tr>  

  <tr><td><b>CUSTID</b></td><td>Identificação do cliente</td></tr>
  <tr><td><b>BALANCE</b></td><td>Saldo para fazer compras</td></tr>
  <tr><td><b>BALANCEFREQUENCY</b></td><td>Frequencia que o saldo é atualizado (1 = frequente, 0 = não frequente)</td></tr>
  <tr><td><b>PURCHASES</b></td><td>Quantidade de compras realizadas</td></tr>
  <tr><td><b>ONEOFFPURCHASES</b></td><td>Quantidade de compras feitas "de uma só vez"</td></tr>
  <tr><td><b>INSTALLMENTSPURCHASES</b></td><td>Quantidade de compras parceladas</td></tr>
  <tr><td><b>CASHADVANCE</b></td><td></td>Dinheiro adinhantado</tr>
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
 





