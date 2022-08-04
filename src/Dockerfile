# Indicando a imagem base e a tag garantido desse modo a idempotência
FROM node:16.15.0

# Indicando a pasta de trabalho
WORKDIR /app

# Copiando apenas os ficheiros de dependências
COPY package*.json ./

# A pasta node_modules é resultado da instalação
RUN npm install	

# Copiando os restantes ficheiros ou pastas para a pasta de trabalho
COPY . .

# As instruções abaixo não entram na camada
# Expondo a porta
EXPOSE 8080 

# Correndo o projecto e só é executado quando é criado o container, 
CMD ["node", "server.js"]
# comando de inicializacao da app