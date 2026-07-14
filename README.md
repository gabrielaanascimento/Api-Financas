
# API de Finanças 💸

Uma API RESTful para gerenciamento de finanças pessoais, desenvolvida com Node.js e Express. O projeto permite registrar transações financeiras (entradas e saídas), consultar saldos atualizados e totais, além de garantir a segurança dos dados através de autenticação por chave de API.

## 🚀 Funcionalidades

- Cadastro, listagem, atualização e exclusão de transações financeiras (CRUD).
- Cálculo automático do saldo atual consolidado.
- Consulta específica para o total de entradas e total de saídas.
- Proteção de rotas utilizando chave de API (`x-api-key`).
- Integração com banco de dados relacional PostgreSQL.

## 🛠️ Tecnologias Utilizadas

- **[Node.js](https://nodejs.org/)**
- **[Express](https://expressjs.com/)** (v5.1.0)
- **[PostgreSQL (pg)](https://node-postgres.com/)**
- **Cors** & **Dotenv**
- **Nodemon** (Ambiente de desenvolvimento)

## ⚙️ Pré-requisitos

Para rodar este projeto localmente, você vai precisar do **[Node.js](https://nodejs.org/)** (que já inclui o gerenciador de pacotes npm) instalado na sua máquina e de um banco de dados **PostgreSQL** devidamente configurado e em execução.

## 📦 Instalação e Execução

1. Clone o repositório para a sua máquina:
   ```bash
   git clone <URL_DO_SEU_REPOSITORIO>
   ````

2. Acesse o diretório do projeto:
```bash
cd api-financas

```


3. Instale as dependências necessárias:
```bash
npm install

```


4. Configure as variáveis de ambiente criando um arquivo `.env` na raiz do diretório com as seguintes chaves:
```env
API_PORT=4000
API_SECRET_KEY=sua_chave_secreta_aqui
DATABASE_URL=postgres://usuario:senha@localhost:5432/nome_do_banco

```


5. Inicie o servidor:
```bash
node server.js

```


**A API estará rodando e disponível no endereço:** http://localhost:4000
**Nota:** Como a API possui proteção de rotas, todas as requisições (exceto a rota raiz `/`) exigem que o cabeçalho `x-api-key` seja enviado com a mesma chave definida em `API_SECRET_KEY` no arquivo `.env` para que os dados sejam processados com sucesso. Certifique-se também de que a tabela `transacoes` está devidamente criada na sua base de dados PostgreSQL.

## 🧪 Scripts Disponíveis

No diretório raiz, você pode executar os seguintes comandos:

* `node server.js`: Inicia o servidor em modo padrão.
* `npx nodemon server.js`: Inicia a API em modo de desenvolvimento, reiniciando o servidor automaticamente sempre que arquivos forem alterados.

## ✒️ Autor

Projeto criado e desenvolvido por **Gabriel Nascimento**.

```

```
