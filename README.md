<div align="center">
<img src="https://user-images.githubusercontent.com/101370736/179435747-a41e7186-b5bf-4f81-a7ac-bd9d8daf04a8.png" height=350 widith=350>
<img src="https://user-images.githubusercontent.com/101370736/179438772-2af80866-731a-4516-aeab-4473d6bf621e.jpeg" height=350 widith=350>
</div>


<h1 align="center">ReactJs - Ignite Lab </h1>

<p align="center">O Ignite Lab foi um projeto da Rocketseat que ocorreu entre os dias 20 e 26 de junho de 2022, focado em ReactJs.
Nesse período, os alunos desenvolveram uma website, apelidado de Event Platform, cujo objetivo é permitir que pessoas se cadastrem em um evento e assistam as aulas dentro da plataforma.
</p>



📌 Acesse a plataforma hospedada no Vercel [clicando aqui](https://ignitelab-reactjs.vercel.app/)

---

## 🚀 Como executar o projeto

### 🔴 Pré-requisitos

<p>

- Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas: [Git](https://git-scm.com), [Node.js](https://nodejs.org/en/).
 
 Além disto é bom ter um editor para trabalhar com o código como [VSCode](https://code.visualstudio.com/). Se você já utilize ele, baixe as seguintes extensões:
 [GraphQL](https://marketplace.visualstudio.com/items?itemName=GraphQL.vscode-graphql),
 [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss),
 [PostCSS Language Support](https://marketplace.visualstudio.com/items?itemName=csstools.postcss)
 </p>
 
###  🛑 Etapas no GraphCMS 🛑

  1. Crie uma conta no [GraphCMS](https://app.graphcms.com/) e clone o schema fornecido pela Rockeseat [clicando aqui](http://rseat.in/lab-graphcms).

  2. Depois de clonar o schema, abra-o e clique em "project setting" (engrenagem). Em seguida, navegue até API Access e copie e salve sua Content API.

  3. Após isso, role a página até a seção "Permanent Auth Tokens", edite seu token e crie 3 novas permissões para o model Subscriber:

      - [x] Create Permission -> Model - All -> Read -> Locales -> All -> Stages -> Published

      - [x] Create Permission -> Model -> Subscriber -> Read -> Stages -> Draft + Published

      - [x] Create Permission -> Model - Subscriber -> Create -> Locales -> All

  4. Copie e salve o value do seu token.


> 😮‍💨 Ufa! Essa parte é importante, pois o token do schema disponiblizado não dispõe previamente dessas permissões. Elas são necessárias para que o cadastro de usuários
possa ser realizado na página Subscribe, além permitir que a página Event tenha acesso as Lessons publicadas!
 
> 😉 Por falar em Lessons, o schema que você clonou está vazio. O que acha de criar uma nova Lesson?

>🤝 Uma dica: Para cadastrar as aulas, você terá que acessar o Content. Agora é com você!

 
 ### 🎲 Rodando a aplicação
 
 **Clone esse repositório**
 ```bash
 $ git clone https://github.com/alissonlimabr/Ignitelab-reactjs
 ```


**Abra o projeto em seu editor de código (preferível VSCode). Em seguida, inicie o terminal e acesse a pasta da aplicação**
 ```bash
$ cd event-plataform
 ```

**Crie seu arquivo DotEnv com o nome ".env.local" na raiz da pasta. Depois, insira as seguintes informações no corpo do arquivo:**
 ```bash
VITE_API_URL="suaContentAPI"
VITE_API_ACCESS_TOKEN="seuToken"
 ```

**Instale as dependências do projeto**
 ```bash
$ npm install
 ```
 
**Execute o a aplicação**
 ```bash
$ npm run dev
 ```

**Pronto! A aplicação será aberta na porta 3000. Acesse:**
 ```bash
http://localhost:3000
 ```

### 🛠 Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:

-   **[ReactJS](https://pt-br.reactjs.org/)**
-   **[React Router Dom](https://github.com/ReactTraining/react-router/tree/master/packages/react-router-dom)**
-   **[GraphQL Code Generator](https://www.graphql-code-generator.com/)**
-   **[TypeScript](https://www.typescriptlang.org/pt/)**
-   **[GraphCMS](https://graphcms.com/)**
-   **[Appolo](https://www.apollographql.com/)**
-   **[Vercel](https://vercel.com/)**
-   **[Vite](https://vitejs.dev/)**


