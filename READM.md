# 💬 ChatGPT FullStack + DevOps

[![Docker Build](https://img.shields.io/badge/Docker-Build-blue)](https://www.docker.com/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

Aplicação FullStack inspirada no ChatGPT, utilizando Node.js, Express, React.js, MongoDB Atlas e infraestrutura DevOps moderna com Docker Compose.

🚀 Deploy instantâneo:

[![Deploy on Render](https://img.shields.io/badge/Deploy-Render-blue?logo=render)](https://render.com/)

---

## 📸 Demonstração

> **Em breve:** Insira aqui um GIF ou uma imagem do funcionamento do app.

---

## ✨ Features

- ✅ Autenticação segura de usuários
- ✅ Upload de arquivos com preview
- ✅ Chat interativo no estilo GPT
- ✅ Painel de Administração de usuários/mensagens
- ✅ Backend e Frontend containerizados com Docker
- ✅ MongoDB Atlas seguro e escalável
- ✅ Ambiente de desenvolvimento e produção separados

---

## 🛠️ Tecnologias Usadas

- **Frontend:** React.js, Vite, TailwindCSS
- **Backend:** Node.js, Express.js, Mongoose
- **Database:** MongoDB Atlas (nuvem)
- **Infraestrutura:** Docker, Docker Compose, PM2
- **Deploy:** Render, Vercel ou VPS pessoal

---

## 🚀 Como Rodar Localmente

### 1. Deploy Tradicional (Sem Docker)

**Backend:**

```bash
cd backend
npm install
npm start
Frontend:

bash
Copiar
Editar
cd frontend
npm install
npm start
Acesse: http://localhost:3000

2. Deploy com Docker Compose
Comando Único:

bash
Copiar
Editar
docker-compose up --build
Acesse: http://localhost:3000

Usando Makefile (opcional):

bash
Copiar
Editar
make up
⚙️ Configuração de Ambiente
backend/.env

env
Copiar
Editar
MONGO_URI=Sua_string_conexao_mongodb_atlas
PORT=5000
frontend/.env

env
Copiar
Editar
VITE_API_URL=http://localhost:5000
🏗️ Estrutura do Projeto
lua
Copiar
Editar
/
|-- backend/
|   |-- controllers/
|   |-- models/
|   |-- routes/
|   |-- uploads/
|   |-- Dockerfile
|   |-- .env
|
|-- frontend/
|   |-- src/components/
|   |-- public/
|   |-- Dockerfile
|   |-- .env
|
|-- docker-compose.yml
|-- Makefile
|-- README.md
|-- .gitignore
📖 API Reference (Principais Endpoints)
POST /api/login → Autenticação de usuários

POST /api/upload → Upload de arquivos

POST /api/message → Enviar mensagens do chat

GET /api/users → Listar usuários (admin)

🛡️ Segurança
Autenticação com JWT.

Banco de dados protegido com IP Whitelisting no MongoDB Atlas.

Deploy seguro HTTPS (caso use Vercel/Render).

🧠 Melhorias Futuras
Integração com API real da OpenAI.

Upload para AWS S3 em vez de local.

Cache Redis para sessões.

📜 Licença
Este projeto está licenciado sob a licença MIT.

🙏 Agradecimentos
OpenAI

MongoDB Atlas

Docker

Render

Vite.js


