FROM node:lts-alpine

COPY . /app

WORKDIR /app

RUN npm install vue @vue/cli @vue/cli-service vue-template-compiler
RUN npm install webpack-dev-server --save-dev

EXPOSE 8080