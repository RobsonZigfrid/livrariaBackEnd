# livrariaBackEnd
Projeto para uma Livraria com MVC, Helpers e Autenticação


## Descrição do Sistema

O projeto consiste em uma API RESTful voltada para o gerenciamento de usuários e livros. A API é desenvolvida utilizando Node.js e o framework Express, garantindo desempenho e flexibilidade. O banco de dados utilizado é o PostgreSQL, oferecendo robustez e segurança no armazenamento dos dados.

* *  A aplicação segue a arquitetura MVC (Model-View-Controller), onde:

 - Controllers lidam com as requisições HTTP.
 - Models representam a estrutura dos dados.
 - Views são desnecessárias, pois a aplicação é uma API.
 - Services contêm a lógica de negócios.
 - Helpers fornecem funções auxiliares, como validação e hashing de senhas.

## Requisitos Funcionais

* *  Autenticação de Usuário:
 - Registro de novos usuários.
 - Login de usuários existentes com validação de senha.

* *  Gerenciamento de Livros:
 - Cadastro de livros com título, autor e preço.
 - Consulta de todos os livros cadastrados.

* *  Gerenciamento de Usuários:
 - Consulta de todos os usuários cadastrados.
 - Criação de novos usuários com validação de dados.

## Requisitos Não Funcionais 
Os requisitos não funcionais descrevem as características de qualidade do sistema. Para este projeto, consideramos os seguintes requisitos:
* * Desempenho
O sistema deve processar até 1000 requisições simultâneas, garantindo respostas rápidas e eficientes, mesmo com múltiplas requisições.

* * Segurança
O sistema deve proteger dados sensíveis por meio de criptografia e autenticação de dois fatores, assegurando o armazenamento de senhas com hash e a comunicação segura via HTTPS.

* * Usabilidade
A interface deve ser amigável e intuitiva, com um tempo de resposta inferior a 2 segundos para ações comuns. As respostas da API devem ser claras e as mensagens de erro, compreensíveis.

* * Escalabilidade
O sistema deve ser capaz de crescer horizontalmente, permitindo suportar o aumento do número de usuários sem comprometer o desempenho.

* * Confiabilidade
O sistema deve garantir a segurança dos dados, registrar erros para diagnóstico e ter alta disponibilidade, sendo acessível constantemente com possibilidade de distribuição em múltiplos servidores.

* * Manutenibilidade
O código deve ser bem organizado, facilitando a modificação e evolução do sistema.

* * Testabilidade
O sistema deve permitir testes automatizados, assegurando a qualidade e estabilidade durante o desenvolvimento.

## Rotas e Funcionalidades

* * Rota de Autenticação (/auth)
POST /register: Criação de novo usuário.
POST /login: Login de usuário.

* * Rota de Livros (/livros)
GET /livros: Lista todos os livros.
POST /livros: Criação de novo livro.

* * Rota de Usuários (/users)
GET /users: Lista todos os usuários.
POST /users: Criação de novo usuário.

* *  Dependências
dotenv: Gestão de variáveis de ambiente (embora não esteja presente no código, é uma prática recomendada).
Express: Framework para a API.
pg: Cliente PostgreSQL.
crypto: Para hashing de senhas.

## Conclusão

Este projeto implementa uma API para o gerenciamento de livros e usuários, com foco em uma autenticação segura. A adoção da arquitetura MVC (Modelo-Visão-Controlador) propicia uma maior organização e facilita a manutenção e a escalabilidade do sistema. A seguir, apresentamos uma visão geral dos principais componentes e funcionalidades do projeto. Para informações detalhadas, consulte a documentação interna.