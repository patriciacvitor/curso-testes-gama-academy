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

- No cmd rodamos o npm start:
$   npm start
Isso vai levantar a aplicação na porta 3000, como indicado no arquivo www.js contido na pasta bin:
    var port = normalizePort(process.env.PORT || '3000');

- No browser digite: localhost:3000

- Se quiser você pode mudar o título que aparece na página no arquivo routes/index.js na linha:
    res.render('index', { title: 'Express' });
    - Onde está escrito " 'Express' ", coloque seu nome, por exemplo.
    - No cmd digite o comando npm start novamente para reiniciar o servidor (o nodemon faria o reload automaticamente).

- Temos também a rota users para obter resposta. No browser digite: localhost:3000/users
    - Essa rota responde "respond with a resource" de acordo com a linha de código:
    res.send('respond with a resource');

-----------------------------------------------------------------------------------------------------

Nessa aula vamos fazer uma classe mockada (existe um conceito chamado Mock). Você mocka um dado que vai retornar do banco de dados para poder fazer os seus testes.

- No VS Code crie a pasta models na raiz da pasta do projeto.

- No cmd:
    - Digite Ctrl + C para parar a execução do node se ainda não tiver feito isso.

    - Instale a suíte de testes Jasmine:
        - https://jasmine.github.io/setup/nodejs.html
        - $   npm install --save-dev jasmine
    - Verifique se no arquivo package.json está instalado o Jasmine em "devDependencies".
    - Verifique se está instalado com o comando $   jasmine init (ele inicializa um projeto criando o diretório spec e um arquivo JSON com a configuração).
    - Se der erro, é porque não está instalado globalmente. Você pode:
        - Instalar globalmente usando -g:
        $   npm install -g --save-dev jasmine
        - Ou rodá-lo diretamente do diretório onde está instalado com:
        $   ./node_modules/jasmine/bin/jasmine.js init
        ou
        $   npx jasmine init

    - Para rodar a aplicação:
        $   jasmine ci
        ou
        $   jasmine
        - Se estiver instalado apenas localmente rode com:
        $   ./node_modules/jasmine/bin/jasmine.js

- O arquivo spec/support/jasmine.json lê o diretório chamado spec e, dentro desse diretório, qualquer arquivo que tiver o nome [sS]pec.js vai ser lido, e qualquer helper que tiver extensão JS, ele vai entender que é um helper criado para usar diretamente no spec.

- Crie um novo diretório (pasta) chamado "models" dentro de spec (clique na pasta spec para garantir que não está dentro da pasta support e crie a pasta models).

- Crie um novo arquivo chamado "cliente.spec.js" dentro de spec/models (clique na pasta models para garantir que está nela).

[------------------------------------- EXTRA ------------------------------------------

    UM POUCO SOBRE PADRÕES DE ARQUITETURA WEB - MONOLÍTICAS E MICRO SERVIÇOS:
    https://lgertel.medium.com/padr%C3%B5es-de-arquitetura-web-monol%C3%ADtica-ou-micro-servi%C3%A7os-7b3f0c9394fe

]

