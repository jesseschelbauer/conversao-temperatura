FROM node:20.11.0-alpine3.19
WORKDIR /app
COPY package*.json .
RUN npm install 
COPY . .
EXPOSE 8080
ENTRYPOINT [ "node", "server.js" ] 