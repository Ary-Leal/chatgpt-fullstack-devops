# Usa Node.js official
FROM node:20

# Cria diretório de app
WORKDIR /app

# Copia os arquivos
COPY package*.json ./
RUN npm install
COPY . .

# Expõe a porta do backend
EXPOSE 5000

# Commando para rodar o servidor
CMD ["npm", "start"]

