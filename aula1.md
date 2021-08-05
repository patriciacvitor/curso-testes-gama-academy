-------------------- O QUE, POR QUE E COMO TESTAR? --------------------

Professor: Danilo Aparecido
Analista, programador, arquiteto de software
Youtuber at Torne-se um Programador

TDD - Testes Unitários
BDD - Testes de Comportamentos
TDD e BDD são processos essenciais para integração e deploy contínua.

TDD = Test Driven Development
Os testes serão os guias do seu desenvolvimento e te ajudar a criar pequenas funções para seu sistema.
É voltado para os desenvolvedores (que estão fazendo todas as features).
Você pensa no problema, desenvolve um robô para simular aquele erro, e desenvolve sua feature baseado no que o robô disse que estava errado.

Exemplo de feature de teste (pequenos pedaços de código):
- Validação de CPF.

BDD = Behavior Driven Development
Está relacionado com os comportamentos que o sistema tem.

Exemplo de feature de comportamento (mais voltado para a área de negócios):
- Um formulário de cadastro que, após ser preenchido, deve retornar o resultado de que foi concluído com sucesso. São uma série de ações que se tornam um conjunto que é uma feature para esse comportamento.

Quando falamos de CI/CD (Continuous Integration/Continuous Delivery), os primeiros passos da nossa pipeline são TDD e BDD.
1º passo: fazer todo o build do seu sistema. Baixar e instalar seu código.
2º passo: rodar os testes unitários. Todos os testes de funções e API's.
2º passo: rodar testes de comportamento.

Tanto TDD como BDD podem ser usados para testar algumas API's, testes de controles.





