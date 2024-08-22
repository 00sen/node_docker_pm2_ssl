# Usa una imagen base de Node.js
FROM node:alpine3.19

RUN mkdir -p /home/node/node-app

COPY . /home/node/node-app

WORKDIR /home/node/node-app

RUN npm install -g pm2
RUN npm install 

CMD ["pm2-runtime","start", "app.js"]
