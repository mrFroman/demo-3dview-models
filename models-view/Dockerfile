FROM node:16.13.0

#LABEL maintainer="estoy@moviendo.me"

RUN npm -g config set user root

RUN npm install -g expo-cli

WORKDIR /app

ENV NODE_ENV development

COPY app.json yarn.lock package.json  /app/
RUN yarn install

CMD ["yarn", "start"]
