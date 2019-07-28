FROM node:lts-alpine

COPY . /app

WORKDIR /app

RUN npm install -g vue @vue/cli @vue/cli-service vue-template-compiler vuex webpack-dev-server

EXPOSE 8080