FROM node:21-alpine

WORKDIR /backend

COPY package*.json ./

RUN npm ci

COPY . .

COPY .env.sample .env

EXPOSE 5000

CMD [ "npm", "start" ]