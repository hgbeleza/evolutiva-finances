FROM node:18-alpine

# Define o diretório de trabalho dentro do container
WORKDIR /app

# Copia os arquivos do frontend para dentro do container
COPY ./frontend .

# Instala as dependências do Angular
RUN npm install && npm run build

# Expõe a porta 4200 (onde o Angular roda)
EXPOSE 4200

# Comando para rodar o frontend
CMD ["npm", "start"]
