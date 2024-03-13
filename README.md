# DesafioDeCodigoDIO

1

Neste desafio, você deve criar um sistema de gerenciamento de usuários que permita adicionar e listar usuários. Você tem a opção de implementar o padrão Singleton para garantir que haja apenas uma instância do gerenciador de usuários em toda a aplicação. No entanto, a implementação do padrão Singleton é opcional e você pode optar por seguir uma abordagem diferente para resolver o desafio, se preferir.

Especificações do Desafio:

Crie uma classe User com os seguintes atributos: id (inteiro) e name (string).
Implemente uma classe UserManager que siga o padrão Singleton. Esta classe deve possuir as seguintes funcionalidades:
a. Adicionar um novo usuário ao sistema, recebendo o nome como entrada.
b. Listar todos os usuários cadastrados.
No programa principal (main), siga as etapas abaixo:
a. Solicite ao usuário a quantidade de usuários que deseja cadastrar.
b. Peça ao usuário para informar os nomes dos usuários, um por linha.
c. Após receber os nomes e cadastrar os usuários, liste os usuários cadastrados.
Entrada
Um número inteiro representando a quantidade de usuários que o usuário deseja cadastrar.

Para cada usuário a ser cadastrado, uma string contendo o nome do usuário.

Saída
Uma lista com os nomes dos usuários cadastrados.

Exemplos
A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

Entrada	
2
Ada
Linus

Saída	
1 - Ada
2 - Linus

Entrada	
3
Grace
Alan
Steve

Saída	
1 - Grace
2 - Alan
3 - Steve

Entrada	
4
Tim
Margaret
John
Richard	

Saída
1 - Tim
2 - Margaret
3 - John
4 - Richard

  
      

2


Descrição

Você foi designado para criar uma calculadora simples em Java, aplicando o padrão de projeto Strategy para representar as operações matemáticas.

Entrada
O programa deve solicitar ao usuário dois números e a operação desejada. As operações podem ser especificadas pelos seguintes sinais: + para soma, - para subtração, * para multiplicação e / para divisão. O usuário deve inserir o sinal correspondente à operação desejada.

Saída
A calculadora deve utilizar o padrão Strategy para realizar a operação escolhida e exibir o resultado.

Exemplos
A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

Entrada	
100
10
/

Saída
10.0

Entrada
9
4
*
Saída
36.0

Entrada
4
3
+

Saída
7.0


3

Descrição
Você deve aprimorar o sistema de monitoramento de produtos, adicionando a capacidade de exibir uma mensagem específica para cada usuário quando um novo produto é adicionado ao catálogo. Além disso, implemente a funcionalidade de permitir que os usuários cancelem sua assinatura para deixar de receber notificações sobre novos produtos.

Entrada
O programa deve solicitar ao usuário que insira o nome do usuário para realizar a ação desejada.
Se o usuário deseja cancelar a assinatura, ele deve digitar "cancelar". Se desejar receber notificações, deve digitar qualquer outro valor.
Se o usuário optar por adicionar um novo produto, será solicitado o nome do produto a ser adicionado.
Saída
Após cada ação, o programa deve exibir mensagens informativas para indicar se a assinatura foi cancelada com sucesso, se o usuário ainda está assinando notificações ou se o produto foi adicionado ao catálogo.

Exemplos
A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

Entrada	

TV
Smart
999
S
Saída	

Notificacao recebida: Novo produto adicionado - TV

Entrada

Smartphone
Apple
3000
S	

Saída

Notificacao recebida: Novo produto adicionado - Smartphone

Entrada

Mouse
Sem fio
340
N

Saida

Programa Encerrado.



4

Descrição

Você está desenvolvendo um sistema simples de carrinho de compras. O desafio é implementar a funcionalidade de calcular o total da compra, permitindo que o usuário escolha entre diferentes estratégias de desconto, utilizando o padrão de projeto Strategy.

Entrada
O programa deve permitir que o usuário adicione produtos ao carrinho, informando o nome e o preço de cada produto. Em seguida, o usuário deve escolher a estratégia de desconto desejada entre duas opções: 10% de desconto ou frete grátis.

Saída
O programa deve calcular e exibir o total da compra com base na estratégia de desconto escolhida.

Exemplos
A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

Entrada

Livro
45
1
	
Saída

Total da compra: R$40.5

Entrada

Air Fryer           
200
2	

Saida

Frete gratis aplicado
Total da compra: R$200.0

Entrada

Celular
1000
1	

Saida

Total da compra: R$900.0

 
5


Descrição

O padrão de projeto Adapter é um padrão de projeto estrutural que permite que objetos com interfaces incompatíveis trabalhem juntos. Ele atua como um intermediário, adaptando a interface de uma classe para outra interface esperada pelo cliente.

Neste desafio, você deverá implementar um conversor de moedas que permitirá que valores monetários sejam convertidos de dólares americanos (USD) para euros (EUR). Embora exista uma taxa de conversão direta de 1 USD = 0.85 EUR, o nosso sistema inicialmente só suportava a conversão de USD para libras esterlinas (GBP). Utilizando o padrão Adapter, você deve adaptar esse sistema antigo para fornecer a nova funcionalidade de conversão direta para EUR, usando a conversão intermediária para GBP.

Entrada
Um valor em dólares americanos USD (Double).

Saída
O valor convertido para euros EUR (Double) usando o adaptador.

Taxa de conversão direta (para referência):
1 USD = 0.85 EUR

Taxas de conversão para a adaptação:
1 USD para GBP = 0.80
1 GBP para EUR = 1.0625

Exemplos
A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

Entrada	

200

Saída

USD: 200.0
EUR: 170.0

Entrada

150

Saída

USD: 150.0
EUR: 127.5

Entrada

1000.0

Saída

USD: 1000.0
EUR: 850.0


Nota:
O padrão Adapter é uma ferramenta valiosa para lidar com incompatibilidades de interface e integrar componentes heterogêneos. No entanto, é importante avaliar cuidadosamente sua utilização para garantir que os benefícios superem os possíveis custos em termos de complexidade e desempenho.

Caso queira saber mais sobre o Design Pattern Adapter:
https://refactoring.guru/pt-br/design-patterns/adapter






 
