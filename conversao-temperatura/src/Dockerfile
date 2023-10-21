#  escolher imagem base
FROM node:18.17.0
# diretorio de trabalho
WORKDIR /app
# pegar os alementos necessários para a execução da imagem
COPY package*.json ./
# baixar todas as deps dentro da imagem
RUN npm install
#copiar todos os outros arquivos necessarios para executar a aplicaçaõ
COPY . .
#especificar que a imagem precisa de uma porta para executar a aplicacao
EXPOSE 8080
#intrução de inicializao do container
CMD ["node", "server.js"]
