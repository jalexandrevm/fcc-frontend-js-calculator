# Calculadora JavaScrip by Alex Marques

Neste projeto, desenvolvi uma calculadora simples com apenas as 4 operações básicas de somar, subtrair, multiplicar e dividir.  

Dentre todas as tecnologias disponíveis, acabei escolhendo usar diretamente o HTML mais o BootStrap (CSS) e um pouco de JavaScript.  

Sei que poderia ter feito tudo usando o JavaScript com o React para criar todos os componentes e posteriormente posicioná-los com o SASS, mais o Redux para usar um repositório único com os valores e as operações adicionadas para depois calcular a senteça.  

Porém, escolhi seguir a ideia do TDD, Test Drivem Development ou Desenvolvimento Dirigido ao Teste, e comecei criando toda a estrutura com o BootStrap usando muitas `<div>'s` para criar toda a **Grid** da calculadora.  

A parte lógica da calculadora se resume a 5 funções que reagem ao evento `onclick()` gerado pelos elementos da calculadora, que seriam:  

- addNumber(num)
- addDecimal()
- addOper(oper)
- clearAll()
- calculate()

A execução do `addOper(oper)` acabou sendo a mais complicado devido às exigências ao operador "-" que em alguns casos deveria ser tratado com uma mudança de sinal ao número digitado.  

O cálculo da expressão completa, com a função `calculate()`, acabou ficando bem simples após o tratamento correto dos valores a serem incluídos no histórico.  

A função `addDecimal()` só teve uma condição a ser tratada que foi a de não incluir mais de um decimal no display da calculadora.  

