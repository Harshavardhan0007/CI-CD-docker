FROM node:current-alpine3.23

WORKDIR /app

COPY package*.json . 

RUN npm install

COPY . .

ENV MONGO_URI=mongodb://mongo:27017/todos

EXPOSE 4000

CMD ["node","server.js"]


