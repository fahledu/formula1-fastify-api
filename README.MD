# Fórmula 1 Minimal API com Node.js e Fastify 🚀

Este projeto fornece uma API minimalista que permite acessar informações sobre equipes e pilotos da Fórmula 1. Ele utiliza **Node.js** e **Fastify**, com suporte a **CORS** para facilitar o consumo em diferentes origens.

---

## 📋 Funcionalidades

- **Listar equipes**: Retorna todas as equipes da Fórmula 1.
- **Listar pilotos**: Retorna todos os pilotos da Fórmula 1.
- **Detalhes do piloto**: Busca informações detalhadas de um piloto por ID.
- **Detalhes da equipe**: Busca informações detalhadas de uma equipe por ID.

---

## 📂 Estrutura do Projeto

```plaintext
├── index.js          # Código principal da API
├── package.json      # Configurações do projeto e dependências
├── tsconfig.json     # Configurações do TypeScript (caso utilizado)
├── .gitignore        # Arquivos/diretórios ignorados pelo Git
├── .env              # Variáveis de ambiente
└── .github/assets    # Imagens e logotipos do projeto
```

---

## 🛠️ Tecnologias

### 📦 Dependências

- **[Fastify](https://www.fastify.io/)** - Framework web rápido e eficiente.
- **[@fastify/cors](https://www.fastify.io/docs/latest/Reference/CORS/)** - Plugin para habilitar CORS no servidor.
- **[TypeScript](https://www.typescriptlang.org/)** - Superset de JavaScript para desenvolvimento escalável (opcional).

### ⚙️ Scripts Disponíveis

- `npm run dist`: Compila o código para a pasta `dist`.
- `npm run start:dev`: Inicia o servidor em modo de desenvolvimento.
- `npm run start:watch`: Inicia o servidor em modo de desenvolvimento com reload automático.
- `npm run start:dist`: Compila e executa a versão empacotada do servidor.

---

## 🚀 Como Executar

### Pré-requisitos

- **[Node.js v20+](https://nodejs.org/)**  
- **[NPM v10+](https://www.npmjs.com/)**

### Passo a Passo

```bash
# Clone o repositório
git clone https://github.com/fahledu/formula1-fastify-api.git

# Acesse o diretório do projeto
cd formula1-fastify-api

# Instale as dependências
npm install

# Inicie o servidor
npm run start:dev
```

---

## 🔌 Endpoints Disponíveis

1. **Listar equipes**  
   - **URL**: `/teams`  
   - **Método**: `GET`  
   - **Resposta**: Lista de todas as equipes.  

2. **Listar pilotos**  
   - **URL**: `/drivers`  
   - **Método**: `GET`  
   - **Resposta**: Lista de todos os pilotos.  

3. **Buscar piloto por ID**  
   - **URL**: `/drivers/:id`  
   - **Método**: `GET`  
   - **Parâmetro**: `id` (string)  
   - **Resposta**: Detalhes do piloto ou mensagem de erro.  

4. **Buscar equipe por ID**  
   - **URL**: `/teams/:id`  
   - **Método**: `GET`  
   - **Parâmetro**: `id` (string)  
   - **Resposta**: Detalhes da equipe ou mensagem de erro.  

---

## 📄 Licença

Este projeto está sob a licença [MIT](LICENSE).  

---

Feito com ❤️ por [fahledu](https://github.com/fahledu/). Contribuições são bem-vindas! 😊