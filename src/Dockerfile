 FROM ubuntu:20.04
 ARG NODE_MAJOR=20
 RUN apt-get update && \
     apt-get install -y curl && \
     curl -fsSL https://deb.nodesource.com/setup_${NODE_MAJOR}.x | bash - && \
     apt-get install -y nodejs && \
     node -v && \
     npm -v
 WORKDIR /app
 COPY . .
 RUN npm install 
 ENTRYPOINT [ "node", "server.js" ] 