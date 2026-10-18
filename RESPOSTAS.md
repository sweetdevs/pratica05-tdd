# Respostas da Reflexão - Prática 05 TDD

1. No Ciclo 1 usamos return 70. Por que isso é aceitável no TDD? O que
obrigou a escrever a soma de verdade?
R: É aceitável pela técnica "fake it", permitindo obter um teste verde rapidamente. O que forçou a escrita da soma real foi o teste de triangulação do Ciclo 2.

2. No Ciclo 3, por que testar com 69 e 70, e não com 50 e 90?
R: Por conta da análise de valor limite, garantindo que o operador `>=` foi aplicado corretamente na fronteira de aprovação.

3. No Ciclo 4, o que mudou na refatoração? Como você teve certeza de
que não quebrou nada?
R: A duplicação de código foi eliminada criando o método `validarNota()`. A certeza de que nada quebrou veio do fato de todos os testes continuarem verdes.

4. No Ciclo 8, por que alteramos os testes antes de mudar o código?
R: No TDD os testes atuam como a especificação. Ao mudar a regra de negócio, ajustamos a especificação primeiro para fazê-la falhar e validar o novo comportamento.

5. Qual ciclo foi o mais difícil para você, e por quê?
R: O Ciclo 7, devido às condições para determinar a menor nota entre A1 e A2 e tratamentos de substituição.
