-------------------- Jasmine I --------------------

CONFIGURAÇÕES INICIAIS:

- Instale o Node para poder usar o NPM para gerenciar pacotes do Node.
Baixe a versão LTS mais recente no site https://nodejs.org/en/download/ e instale.
(Existe também o Yarn, mais novo e também utilizado para instalação de pacotes.)

- Acesse o prompt de comando.
    - Como acessar o prompt de comando do Windows?
        Na barra de ferramentas, no canto inferior esquerdo temos o botão Iniciar do Windows, ao lado dele, na barra de pesquisa, digite:
        -  cmd
        -  Clique em Prompt de Comando

- No Prompt de Comando:
    - Verifique se o node está instalado digitando (o $ não deve ser digitado):
        $   node --version
        ou
        $   node -v
        Se estiver instalado corretamente, aparecerá a versão.

    - Você também pode testar se o npm está instalado com:
        $   npm --version
        ou
        $   npm -v

    - Instale o Express Generator:
        - Site: https://expressjs.com/pt-br/starter/generator.html
        - Digite no cmd:
        $   npm install express-generator -g
        ou
        $ npm i -g express-generator
    
    - Verifique, pelo cmd, se o Express está instalado:
        $   express --version

    - Pelo cmd, acesse a pasta onde ficará seu projeto. Basta digitar:
        $   cd caminho_da_sua_pasta_no_computador
        Exemplo: D:\GamaAcademy\projeto-testes

    - No cmd, crie a aplicação digitando:
        $   express tdd_bdd_jasmine_cucumber --view=ejs

    - Acesse a pasta do projeto:
        $   cd tdd_bdd_jasmine_cucumber

    - Instale as dependências:
        $   npm install
        ou
        $   yarn install (caso você use o yarn)

    - Abra a pasta do projeto no VS Code, digitando no cmd:
        $   code .

- No VS Code:
    - Arquivo package.json:
        - O "start", em "scripts", é o que vai guiar a aplicação node JS.
        Se você criar um arquivo teste.js, por exemplo, apenas com console.log('Oi');, e digitar no cmd:
        $   node teste.js
        O node do seu arquivo será executado e a mensagem "Oi" será exibida no seu cmd.

.
.
.
.
.
.
.

[------------------------------------- EXTRA ------------------------------------------

    UM POUCO SOBRE PADRÕES DE ARQUITETURA WEB - MONOLÍTICAS E MICRO SERVIÇOS:
    https://lgertel.medium.com/padr%C3%B5es-de-arquitetura-web-monol%C3%ADtica-ou-micro-servi%C3%A7os-7b3f0c9394fe

]

