# indicando a imagem base
FROM node:16.15.0
# inddicando a pasta de trabalho
WORKDIR /app
# copiando apenas os ficheiros com as dependencias
COPY package*.json ./

# instalando o node , criando a pasta node_modules
RUN npm install	

#copiando os restantes ficheiros ou pastas para a pasta de trabalho
COPY . .
# Expondo a porta
EXPOSE 8080 
# correndo o projecto
CMD ["node", "server.js"]
