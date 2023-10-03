# testeCaixaBrancaTQS

## Descrição
O teste de caixa branca é uma técnica de teste de software que examina o código interno de um programa para avaliar sua lógica, estrutura e caminhos de execução, com o objetivo de encontrar erros e garantir uma cobertura abrangente do código-fonte.

![Descrição](caixaBrancaTQS.png)

 # 1- A DOCUMENTAÇÃO FOI DESCRITA NO CÓDIGO? 
 Não foi descrita no codigo, pois é possivel encontrar alguns erros.

 # 2- AS VARIÁVEIS E CONSTANTES POSSUEM BOA NOMENCLATURA?
Poderia ter nomes mais objetivos onde facilitaria a leitura e compreensão do codigo.

# 3- EXISTEM LEGIBILIDADE E ORGANIZAÇÃO NO CÓDIGO?
Existe ambas, o código esta bem estruturado e seguindo o padrão 

# 4- TODOS OS NULLPOINTERS FORAM TRATADOS?
Todos nullpointers foram tratados

# 5- A ARQUITETURA UTILIZADA FOI DEVIDAMENTE RESPEITADA?
Sim, ela foi devidamente respeitada


# 7- ERROS DO CÓDIGO 
1. Variavel urL nunca usada 
2. Falta de Fechamento de Conexão, onde pode ocorrer diversos problemas
3. " 'newInstance()' is deprecated" significa que ele foi descontinuado em favor de mecanismos mais novos e flexíveis para criar objetos.

![Descrição](caixaBrancaErrosTQS.png)



# 8- GRAFO DE FLUXO
 1. Segue a imagem

![Descrição](GrafoDeFluxo.png) 


# 9- COMPLEXIDADE CICLOMÁTICA

1. V(G) = 11 - 9 + 2 = 4.
2. V(G) = 3 + 1 = 4.
(Utilizando as duas fórmulas é possível identificar o resultado "4", representando 4 caminhos possíveis.)

# 10- BASE DE CAMINHOS

1. Ponto de Entrada -> Início do método conectarBD -> Construção da URL de conexão -> Tentativa de conexão com o banco de dados -> Fim do método conectarBD;

2. Ponto de Entrada -> Início do método verificarUsuario -> Construção da instrução SQL -> Criação da declaração SQL -> Execução da consulta SQL -> Verificação do resultado da consulta (com resultado verdadeiro) -> Definir a variável 'result' como verdadeira e obter o nome -> Retorno da função verificarUsuario;

3. Ponto de Entrada -> Início do método verificarUsuario -> Construção da instrução SQL -> Criação da declaração SQL -> Execução da consulta SQL -> Verificação do resultado da consulta (sem resultado verdadeiro) -> Retorno da função verificarUsuario;

4. Ponto de Entrada -> Início do método verificarUsuario -> Construção da instrução SQL -> Criação da declaração SQL -> Execução da consulta SQL (com erro) -> Tratamento de exceção -> Retorno da função verificarUsuario.

