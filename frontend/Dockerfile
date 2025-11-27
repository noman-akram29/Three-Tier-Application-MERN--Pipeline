FROM node:21-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

COPY .env.sample .env.local

EXPOSE 5173

CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]
