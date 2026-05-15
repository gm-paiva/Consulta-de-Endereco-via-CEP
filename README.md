# 📮 Consulta de Endereço via CEP

> Aplicação web que realiza consultas de endereço a partir de um CEP, utilizando JavaScript no navegador para requisições HTTP à API pública ViaCEP.

---

## 📌 Sobre o Projeto

Esta aplicação permite ao usuário digitar um CEP e obter as informações de endereço correspondentes, como logradouro, bairro, cidade, estado e região. A consulta é feita diretamente no navegador via requisição HTTP à [API ViaCEP](https://viacep.com.br/), e os resultados são exibidos dinamicamente na página, sem recarregamento.

A atividade foi desenvolvida como parte das práticas acadêmicas da **FATEC Jacareí – Faculdade de Tecnologia de Jacareí**, no curso de **Desenvolvimento de Software Multiplataforma (DSM)**.

---

## 🚀 Tecnologias Utilizadas

- [Node.js](https://nodejs.org/) — Ambiente de execução JavaScript no servidor
- [Express v5](https://expressjs.com/) — Framework web para Node.js
- [dotenv](https://github.com/motdotla/dotenv) — Gerenciamento de variáveis de ambiente
- HTML5 + CSS3 — Estrutura e estilização da página
- JavaScript (Fetch API) — Requisições HTTP à API ViaCEP
- [ViaCEP](https://viacep.com.br/) — API pública para consulta de CEPs

---

## 📁 Estrutura do Projeto

```
app/
├── public/
│   ├── assets/
│   │   ├── css/
│   │   │   └── main.css       # Estilos da aplicação
│   │   └── js/
│   │       └── main.js        # Lógica de consulta à API ViaCEP
│   └── pages/
│       └── index.html         # Página principal com campo de busca
├── .env                        # Variáveis de ambiente (porta do servidor)
├── .gitignore
├── package.json
├── package-lock.json
└── server.js                   # Servidor Express
```

---

## 🔀 Rotas Disponíveis

| Método | Rota        | Descrição              |
|--------|-------------|------------------------|
| GET    | `/`         | Página principal       |
| GET    | `/assets/*` | Arquivos estáticos     |

---

## ✨ Funcionalidades

- Consulta de endereço a partir de um CEP digitado pelo usuário
- Validação do CEP antes de realizar a requisição (deve conter 8 dígitos)
- Exibição dinâmica dos dados retornados: CEP, logradouro, complemento, bairro, cidade, UF, estado, região e DDD
- Feedback visual de estados: carregando, sucesso e erro
- Disparo da busca ao pressionar **Enter**
- Limpeza automática do resultado ao apagar o campo

---

## 🔧 Variáveis de Ambiente

Crie um arquivo `.env` na raiz do projeto com a seguinte variável:

```env
PORT=3002  # ou qualquer outra porta de sua preferência
```

> ⚠️ O arquivo `.env` já está no `.gitignore` e **não deve ser versionado**.

---

## ⚙️ Como Executar

### Pré-requisitos

- [Node.js](https://nodejs.org/) instalado (versão 14 ou superior)
- npm (incluído com o Node.js)

### Passo a passo

```bash
# 1. Clone o repositório
git clone https://github.com/gm-paiva/nome-do-repositorio.git

# 2. Acesse a pasta do projeto
cd app

# 3. Instale as dependências
npm install

# 4. Configure as variáveis de ambiente
# Crie um arquivo .env na raiz com o seguinte conteúdo:
PORT=3002

# 5a. Inicie o servidor (produção)
npm start

# 5b. Inicie o servidor (desenvolvimento com hot reload)
npm run dev
```

Acesse no navegador: [http://localhost:3002](http://localhost:3002)

---

## 📚 Contexto Acadêmico

| Campo          | Informação                                        |
|----------------|---------------------------------------------------|
| 🏫 Instituição | FATEC Jacareí                                     |
| 🎓 Curso       | Desenvolvimento de Software Multiplataforma – DSM |
| 📖 Disciplina  | Desenvolvimento Web I                            |
| 👨‍🏫 Professor(a) | [Arley Ferreira de Souza](https://github.com/arleysouza)                          |
| 📅 Semestre    | 1º Semestre - 2026                       |

---

## 👤 Autor

Desenvolvido por **[Guilherme Matos Paiva](https://github.com/gm-paiva)**.

---

## 📄 Licença

Este projeto está sob a licença MIT.
