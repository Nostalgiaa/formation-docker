#FROM node:10-alpine
#RUN mkdir -p /home/node/app/node_modules && chown -R node:node /home/node/app
#WORKDIR /home/node/app
#COPY package*.json ./
#USER node
#RUN npm install
#COPY --chown=node:node . .
#EXPOSE 8080
#CMD [ "node", "app.js" ]

FROM node:14
WORKDIR /app
COPY ./package.json ./
RUN npm install
COPY . .
CMD [ "node", "server.js" ]

#docker run -p 8081:8080 tp3
# ---> Running on http://0.0.0.0:8080
# ---> http://localhost:8081 ----> OK for me !!