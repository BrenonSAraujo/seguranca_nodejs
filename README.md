<p align="center">
<img src="https://github.com/user-attachments/assets/c85f8415-5b75-4294-9758-a498350c1908"/>
<p align="center">
<img loading="lazy" src="http://img.shields.io/static/v1?label=STATUS&message=ABERTO%20PARA%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge" alt="" style="max-width: 100%;"/>
</p>

### Tópicos


- [Descrição do projeto](#descrição-do-projeto)

- [Funcionalidades](#funcionalidades)

- [Ferramentas utilizadas](#ferramentas-utilizadas)

- [Técnicas e Tecnologias Utilizadas](#técnicas-e-tecnologias-utilizadas)

- [Acesso ao projeto](#acesso-ao-projeto)

## Descrição do projeto 

<p align="justify">
 Este projeto simula uma API de um supermercado com suas principais entidades tabeladas, são elas: usuário e produtos. Além disso, neste backend, é feito um relacionamento entre estas entidades, por meio de permissões e roles de usuários e produtos.
</p>

## Funcionalidades

:heavy_check_mark: `Funcionalidade 1:` CRUD na API;

:heavy_check_mark: `Funcionalidade 2:` Validações de formulário;

:heavy_check_mark: `Funcionalidade 3:` Relacionamento entre tabelas;

:heavy_check_mark: `Funcionalidade 4:` Criptografia de informações sensíveis;

:heavy_check_mark: `Funcionalidade 5:` Abstração das operações de banco por meio de um ORM;

:heavy_check_mark: `Funcionalidade 6:` Virtualização do banco de dados por meio de conteiner;


## Ferramentas utilizadas
[![My Skills](https://skillicons.dev/icons?i=nodejs,express,sequelize,docker,)](https://skillicons.dev)

###

## ✔️ Técnicas e Tecnologias Utilizadas

As principais técnicas e tecnologias abordadas são:

- `NodeJS`: permite executar código JavaScript no lado do servidor;
- `Express`: framework de aplicativo web para Node.js que simplifica a criação de aplicativos web e móveis;
- `Sequelize`: ORM que permite a interação com bancos de dados relacionais, como o SQLite escolhido no projeto;
- `JWT`: padrão para autenticação, autorização e troca de informações;
- `UUID`:  permite identificar dados de forma única em sistemas computacionais;
- `Docker`: software de código aberto usado para implantar aplicativos dentro de containers virtuais.


## Acesso ao projeto
  - ``git clone https://github.com/BrenonSAraujo/seguranca_nodejs.git``: Clone o projeto do GitHub para a sua máquina
  
  - ``npm i``: Instale as dependências do projeto
    <p>Foi escolhido virtualizar o banco de dados por meio do Docker. As informações de nome, usuário, senha e banco estão no arquivo config.json. Segue o comando utilizado no terminal: </p>
  - ``docker pull postgres``: baixar a imagem do PostgreSQL
  - ``docker run --name meu-postgres -e POSTGRES_USER=meuusuario -e POSTGRES_PASSWORD=suasenha -e POSTGRES_DB=meubanco -p 5432:5432 -d postgres``: iniciar um container no postgres
    <p>Após isso, siga os passos abaixo para executar as migrações que já constam no projeto:</p>
    
  - ``npx sequelize-cli db:migrate``: para executa as migrações
  
  - ``npx sequelize-cli db:seed:all``: para executar todas as seeds
    
  - ``npm run start``: para rodar a aplicação
    
