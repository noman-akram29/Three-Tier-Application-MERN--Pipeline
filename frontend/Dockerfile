FROM node:21-alpine

WORKDIR /frontend

COPY package*.json ./

RUN npm ci

COPY . .

COPY .env.sample .env

EXPOSE 3000

CMD [ "npm", "run", "dev", "--", "--host", "0.0.0.0" ]