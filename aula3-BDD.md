-------------------- Behavior Driven Development (BDD) --------------------

Exemplos de problemas de comportamento:
- Cores
- Textos
- Entrar numa lugar, clicar em outro
- Ter algum tipo de sessão nesse lugar
- Digitar login e senha
- Onde está o botão
- Disposição da tela

Quem resolvia isso eram pessoas que trabalhavam com teste de qualidade (QA).

-------------------- FERRAMENTAS --------------------

- Selenium:
    - https://www.selenium.dev/
    - Selenium é uma ferramenta que consegue fazer coisas como abrir o browser, escrever o texto em certo local, clicar no botão e mostrar o resultado sozinho.

Teste regressivo: quando há uma grande mudança no sistema, como uma versão 2.0, e todas as features precisam ser retestadas.
Com o Selenium já não era preciso ter várias pessoas testando tudo novamente, bastava uma rodando o Selenium para fazer testes.

- Cucumber (BDD):
    - https://cucumber.io/docs/guides/browser-automation/
    - Trabalha com o Selenium para fazer testes BDD.

- Cypress:
    - https://www.cypress.io/
    - No site diz: "Cypress makes setting up, writing, running and debugging tests easy."
    - Com essa ferramenta é possível, de uma forma simples, fazer o setup da máquina, rodar e fazer tudo funcionar de forma amigável.
    - Faz os testes de BDD.

- Jest:
    - https://jestjs.io/pt-BR/
    - Faz os testes de TDD.

Qual a diferença do Jest para o Jasmine?
No Jest você tem a opção do watch, então você consegue levantar um servidor enquanto faz os testes e ele vai testando de forma automática.