# 🛒 Loja Virtual - Frontend

Este é o repositório **frontend** do projeto **Loja Virtual**, desenvolvido como parte do MVP da Sprint 3. A aplicação permite aos usuários visualizar produtos, adicionar itens ao carrinho e gerenciar pedidos de forma prática e intuitiva.

A interface é desenvolvida em **HTML, CSS (Bootstrap)** e **JavaScript**, consumindo uma API FastAPI no backend para funcionalidades como listagem, edição e exclusão de pedidos.

---

## 📷 Arquitetura da Aplicação

A arquitetura da aplicação foi baseada na separação de responsabilidades entre frontend e backend. O frontend é responsável por:

- Exibir produtos vindos da API externa (Fake Store API);
- Enviar pedidos para o backend;
- Consultar, editar e excluir pedidos já realizados por meio da API local.

### 🔁 Fluxo de Funcionamento

![imagem_fluxograma_projeto](./img/Fluxograma%20Software.jpg)
---

## ⚙️ Instalação e Uso

Siga as etapas abaixo para rodar o frontend localmente.

### ✅ Pré-requisitos

- Navegador web moderno (Google Chrome, Firefox, etc.)
- Editor de código (Visual Studio Code, por exemplo)
- Backend da aplicação em execução (FastAPI)
- Servidor local como o **Live Server** do VSCode (recomendado)

### 📦 Estrutura de Diretórios

frontend/ 
    ├── app/ 
_______├── static/ 
_____________├── order_manager.js
_____________├── script.js
_____________├── style.css
_______├── index.html 
_______├── order_manager.html
_______├── app.py
_______├── Dockerfile
_______├── Docke-compose
_______├── requirements.txt
_______└── README.md

## ▶️ Passos para execução local

### 1. Crie uma pasta e clone o repositório abaixo: (esse repositório deve estar na mesma pasta junto ao repositório do back-end)

### 2. Clone este repositório:

```bash
git clone https://github.com/victorazevedo0/MVP_Sprint-3_Front-end.git
```

### 3. Abra o projeto no Visual Studio Code (ou editor de sua preferência) acessando a pasta que você criou (onde já possui ou possuirá o também o repositório do back-end).

```bash
cd [pasta_que_voce_criou] > MVP_Sprint-3_Front-end
```
   
### 4. Execute com o **Live Server** clicando com o botão direito sobre index.html e escolhendo "Open with Live Server".

Obs: **Certifique-se de que o backend (FastAPI) está rodando. (como informando no README.md do backend)**

## 🛠️ Tecnologias Utilizadas

    HTML5
    CSS3 (Bootstrap 5)
    JavaScript
    FastAPI (backend - API)
    FakeStore API (catálogo de produtos)

## ✨ Funcionalidades

    Listagem de produtos disponíveis
    Adição ao carrinho e finalização de pedidos
    Visualização de pedidos existentes
    Filtro por status e e-mail
    Edição e exclusão de pedidos via modal

### 📓 Segue documentação da API externa, no qual está sendo utilizada para carregar os produtos da API no projeto através de um GET.

[Fake Store](https://fakestoreapi.com/docs#tag/Products)
Obs: O projeto está com propensão de crescer, com cadastro de produtos, clientes e melhoria na estrutura de pedidos.

## ⚙️ Rodando o projeto via Docker

### 1. Crie uma pasta e clone o repositório abaixo: (esse repositório deve estar na mesma pasta junto ao repositório do back-end)

### 📥 2. Clone o Repositório

```bash
git clone https://github.com/victorazevedo0/MVP_Sprint-3_Front-end.git
```

### 🐳 3. Instalando o Docker e o WSL2:

📌 Pré-requisitos

Instale o Docker de acordo com seu sistema operacional:

    📥 Windows
    📥 Ubuntu
    📥 MacOS

⚠️ usuários de windows, é importante verificar [se a virtualização de sua máquina está ativada na BIOS de sua máquina](https://support.microsoft.com/pt-br/windows/habilitar-a-virtualiza%C3%A7%C3%A3o-no-windows-c5578302-6e43-4b4b-a449-8ced115f58e1), pois ela é fundamental para habilitação do WSL2. Em seguida, você deve seguir os passos de instalação e habilitação do [WSL2](https://learn.microsoft.com/pt-br/windows/wsl/install), para execução do Docker.


### 4. Acesse a pasta que você criou onde já possui ou possuirá o também o repositório do back-end via Visual Studio Code (ou editor de sua preferência):

```bash
cd [pasta_que_voce_criou] > MVP_Sprint-3_Front-end
```

### Segue estrutura do projeto para rodar via docker:

```
[pasta_que_você_criou]/ 
    ├── MVP_Sprint-3_back-end/ 
____├── MVP_Sprint-3_Front-end 
_____________├── docker-compose.yml
```

### 🧱 🚀 5. Construa a Imagem e Rode o container

E rode o código para contruir as imagens e rodar os containers:

```bash
docker-compose up --build
```
