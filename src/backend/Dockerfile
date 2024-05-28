# Use a imagem Node.js como base
FROM node:latest

# Diretório de trabalho dentro do contêiner
WORKDIR /usr/src/app

# Instalar dependências do backend
COPY package*.json ./
RUN npm install

# Copiar o código fonte do backend para o contêiner
COPY . .

# Expor a porta onde o servidor Express irá rodar
EXPOSE 3000

# Comando para iniciar o servidor Express
CMD ["npm", "start"]
