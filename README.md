<p align="center">
  <img src="https://user-images.githubusercontent.com/94487469/233145271-4e81ecdb-fd9c-4dad-aed7-340883fa5b94.png">
</p>

Olá, seja bem vindo ao repositório do projeto Trybesmith! Aqui você irá aprender como instalar e testar esse projeto na sua máquina, para desfrutar das mais diversas funções que esse projeto possui. Eu criei uma loja de itens medievais em formato de API utilizando Typescript. Durante o desenvolvimento do projeto, utilizei todas as camadas da aplicação (Models, Service e Controllers) para construir o meu código. Através dessa aplicação, é possível realizar operações básicas de um banco de dados, tais como Criação, Leitura, Atualização e Exclusão (CRUD).

Para a construção da API, criei diversos endpoints que leem e escrevem em um banco de dados utilizando o MySQL. Utilizei o framework Node Express para a construção da API. Com o objetivo de deixar o código mais compreensível e robusto, apliquei tipos nas variáveis e funções utilizadas.

Com essa aplicação, é possível realizar diversas operações, como cadastrar produtos, listar produtos, cadastrar pessoas usuárias, além de possibilitar o login usando JWT. 

## Como usar :computer: :rocket: 

Usando o Thunder Client ou uma ferramenta de sua escolha, você pode testar todas as rotas disponíveis no projeto.

### Requisitos :clipboard: 

Este projeto pode ser executado de duas formas distintas: a primeira exige a instalação do NODE, enquanto a segunda possibilita o uso do Docker para rodar em uma máquina virtual.

### Instalação :wrench:
#### Com docker:

- Rode o serviço `node` e `db` com o comando `docker-compose up -d.`

Lembre-se de parar o `mysql` se estiver usando localmente na porta padrão (`3306`), ou adapte, caso queria fazer uso da aplicação em containers;
Esses serviços irão inicializar um container chamado `trybesmith` e outro chamado `trybesmith_db`;
A partir daqui você pode rodar o container `trybesmith` via CLI ou abri-lo no VS Code.

- Use o comando `docker exec -it trybesmith bash` e sigas passos abaixo.
Ele te dará acesso ao terminal interativo do container criado pelo compose, que está rodando em segundo plano.

- Instale as dependências com `npm install`.

#### Sem docker:

- Instale as dependências com `npm install`

Para rodar o projeto desta forma, obrigatoriamente você deve ter o node instalado em seu computador.

### Configuração :gear:

Depois de instalar as dependências, você vai precisar criar o banco de dados na qual a API vai consumir. para isso, siga os seguintes passos:

- Caso você não tenha optado por usar o docker, você precisa ter o MySQL instalado na sua máquina, caso contrário, o container já está configurado.
Eu recomendo a utilização da extensão do VScode `Database Client`. Ela ajuda a manipular e visualizar os dados do banco. Outra ferramenta é o MySQL Workbench, fica a seu critério. :smiling_face_with_smiling_eyes:

- Depois disso, você vai notar um arquivo no repositório desse projeto chamado `trybesmith.sql`. Ele cria o banco e as tabelas ao mesmo tempo que o popula.

- Execute-o. Caso voce tenha a extensão `Database Client`, basta selecionar todo o conteúdo do arquivo e apertar (`Ctrl+Enter`).
Observe abaixo o Diagrama de Entidade-Relacionamento do banco que você acabou de criar:


<img width="988" alt="diagram-der" src="https://user-images.githubusercontent.com/94487469/233140288-574a366c-f9ee-46ab-9dbd-37323d7ee4d1.png">


### Execução :runner:

Depois de instalar as dependências, basta rodar o comando `npm run dev` para o server ficar online e você poderá fazer requisições a vontade. Sugiro utilizar o `Thunder Client` ou alguma outra ferramenta de sua escolha. 
exemplo de rota do projeto: `http://localhost:3000/products`

## Contato :telephone_receiver:

Caso você tenha alguma dúvida sobre esse projeto ou queira da um feedback você encontra minha redes sociais no meu portifólio clicando [aqui](https://felupee.github.io/#contact).
