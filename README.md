# inf-21-dw2-g05

Mysql
Inicialização

    Começou-se por instalar my sql(workbench) no computador e de seguida o servidor foi instalado;
    Configuração da base de dados: pasta API/config/db.config.js

Criação do schema

    Um schema novo foi criado no servidor que acabou de ser criado com o nome de usersdb e clicou-se em apply.

Criação da base de dados

    Depois da nova base de dados estar criada no schema uma nova tabela com o nome de usertab foi criada.

Criação das tabelas

    Começamos por criar a primeira coluna com o nome de id com um datatype de INT, PK(primary key) e NN(not null)
    Depois criamos a segunda coluna com o nome de name, com um datatype de VARCHAR(45), ou seja um campo que pode conter letras e números até 45 caracteres, também NN
    De seguida outra coluna foi criada com o nome de lastName e com um datatype de VARCHAR(45).
    Foi criada outra coluna com o nome de age, com um datatype de INT.  
    Depois a database foi conectada à api.
    O script de criação e inserção estão dentro do ficheiro users na pasta routes.


API

    Recurso utilizadores
    Para a API foram utilizados os packages expressI e o Mysql.
    Criamos a rota de users com os seguintes endpoints:
    /users - Get para apresentar todos os utilizadores;
    /users - Post para a criação de um novo utilizador;
    /users/:id - Get para procurar informações sobre o utilizador através do seu id;
    /users/:id - Delete recebendo o id do utilizador como parâmetro para apagar um utilizador em específico;
    /users - Patch para poder atualizar os parâmetros de um utilizador em específico escolhido através do id;
    
    Recurso posts dos utilizadores
    Para a API foram posts os packages expressI e o Mysql.
    Foi criada a rota de posts com os seguintes endpoints:
    /posts - Get para apresentar todos os posts;
    /posts - Post para a criação de um novo post;
    /posts/:id - Get para procurar informações sobre o post através do seu id;
    /posts/:id - Delete recebendo o id do post como parâmetro para apagar um post em específico;
    /posts - Patch para poder atualizar os parâmetros de um post em específico escolhido através do id;
    
    
Autenticação

    Para esta ser feita foi necessário criar uma auth aplication no github e obter credencias que depois foram colocadas no ficheiro com código.

React APP

    Para criar a react app foi necessário criar uma pasta nova. Nesta há outras pastas tais como a Components aonde estão todos os componentes necessários para a       criação de um ui. Nesta app são apresentados os utilizadores com id nome, apelido e idade estes são adicionados à base de dados usersdb à tabela usertab.
    
    A React APP tem os seguintes endpoints
    /create para criar utilizadores na base de dados;
    /users para apresentar os utilizadores na base de dados;
    /update para atualizar a idade dos utilizadores na base de dados;
    /delete/:id para apagar um utilizador sabendo o seu id na base de dados;
