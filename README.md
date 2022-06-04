# inf-21-dw2-g05



API

Para a API forma utilizados os packages expressI e o Mysql.
Criamos a rota de users com os seguintes endpoints:
/users - Get para apresentar todos os utilizadores;
/users - Post para a criação de um novo utilizador;
/users/:id - Get para procurar informações sobre o utilizador através do seu id;
/users/:id - Delete recebendo o id do utilizador como parâmetro para apagar um utilizador em específico;
/users - Patch para poder atualizar os parâmetros de um utilizador em específico escolhido através do id; 

Todo o código utilizado na criação dos endpoints da API está numa pasta denominada Controllers no ficheiro users.js sendo o código de cada endpoint exportado posteriormente para a pasta routes nomeadamente no ficheiro users.js.
