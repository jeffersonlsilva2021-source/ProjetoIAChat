# 🤖 Assistente Virtual com IA

Projeto Final da Situação de Aprendizagem do curso **IACHAT - SENAI**.

O objetivo é desenvolver um **Assistente Virtual Inteligente** utilizando a API da OpenAI, com uma interface web e uma API em Node.js responsável por processar as mensagens.

---

## 📋 Objetivo

Desenvolver um chatbot que permita ao usuário conversar com uma Inteligência Artificial através de uma interface web.

A aplicação deve possuir:

- Front-end em HTML, CSS e JavaScript;
- Back-end em Node.js utilizando Express;
- Integração com a API da OpenAI;
- Comunicação utilizando Fetch API.

> **Importante:** Não será utilizado banco de dados neste projeto.

---

# 🛠 Tecnologias

## Front-end

- HTML5
- CSS3
- JavaScript
- Fetch API

## Back-end

- Node.js
- Express
- OpenAI API

---

# 📁 Estrutura sugerida

```
projeto/
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── backend/
│   ├── server.js
│   ├── routes/
│   ├── controllers/
│   ├── .env
│   └── package.json
│
└── README.md
```

---

# ✅ Funcionalidades Obrigatórias

## Interface

- Área de conversa
- Campo de texto
- Botão Enviar
- Botão Nova Conversa

---

## Envio de mensagens

O usuário digita uma mensagem.

O JavaScript envia para a API utilizando Fetch.

A API consulta a OpenAI e retorna a resposta.

---

## Histórico

Durante toda a conversa as mensagens devem permanecer armazenadas.

Exemplo:

```javascript
let messages = [];
```

---

## Nova conversa

Ao iniciar uma nova conversa deve:

- limpar o histórico;
- apagar as mensagens da tela.

---

## Indicador de carregamento

Enquanto a IA responde deverá existir um indicador, como:

- Pensando...
- Carregando...
- Spinner

---

## Tratamento de erros

Caso a API apresente algum problema, mostrar uma mensagem amigável ao usuário.

Exemplo:

```
Não foi possível obter resposta da IA.
Tente novamente em alguns instantes.
```

---

## Organização visual

As mensagens devem possuir estilos diferentes para:

- Usuário
- Assistente

---

# 🧠 Prompt do Sistema

Antes de enviar qualquer mensagem para a OpenAI, a API deverá incluir um **System Prompt** definindo o comportamento do assistente.

O aluno poderá utilizar um dos cenários sugeridos ou criar um cenário próprio, como:

- Empresa de tecnologia
- Clínica
- Restaurante
- Escola
- Academia
- Pet Shop
- Biblioteca
- Agência de viagens
- Loja virtual

O assistente deve responder apenas sobre o contexto escolhido.

---

# 🌐 API

## POST /chat

### Requisição

```json
{
    "mensagem": "Olá"
}
```

### Resposta

```json
{
    "response": "Olá! Como posso ajudá-lo hoje?"
}
```

---

# 🔄 Fluxo da aplicação

```
Usuário
   │
   ▼
Front-end (HTML/CSS/JS)
   │
Fetch API
   │
   ▼
Node.js + Express
   │
System Prompt
   │
   ▼
OpenAI API
   │
Resposta
   │
   ▼
Front-end
```

---

# 🚀 Como executar

## 1. Clonar o projeto

```bash
git clone <repositorio>
```

---

## 2. Instalar as dependências

```bash
cd backend

npm install
```

---

## 3. Criar o arquivo .env

```env
OPENAI_API_KEY=sua_chave
PORT=3000
```

---

## 4. Executar

```bash
npm start
```

ou

```bash
node server.js
```

---

## 5. Abrir o Front-end

Abra o arquivo:

```
frontend/index.html
```

ou utilize uma extensão como **Live Server**.

---

# ⭐ Funcionalidades Extras (Bônus)

- Documentação da API
- Modo escuro
- Envio com Enter
- Copiar respostas
- Limpar conversa
- Contador de mensagens
- Horário das mensagens
- Scroll automático
- Markdown
- LocalStorage

---

# 📦 Exemplo de resposta da API

```json
{
    "response": "Olá! Em que posso ajudá-lo?"
}
```

---

# 📌 Requisitos

- Node.js 18+
- Conta na OpenAI
- Chave da API
- Navegador moderno

---

# 👨‍🏫 Critérios de avaliação

- Organização do código
- Interface
- Funcionamento da API
- Integração com a OpenAI
- Tratamento de erros
- Boas práticas de programação
- Funcionalidades extras

---

# 📧 Entrega

Enviar:

- Código do Front-end
- Código do Back-end
- README.md

Para:

**jefferson.lopes@sp.senai.br**

---

Curso **IACHAT - SENAI**