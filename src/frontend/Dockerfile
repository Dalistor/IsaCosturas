# Use a imagem Node.js como base
FROM node:latest

# Diretório de trabalho dentro do contêiner
WORKDIR /usr/src/app

# Instalar dependências do frontend
COPY package*.json ./
RUN npm install

# Copiar o código fonte do frontend para o contêiner
COPY . .

EXPOSE 8080

# Comando para compilar e servir o aplicativo Vue.js
CMD ["npm", "run", "serve"]
