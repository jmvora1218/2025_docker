FROM node:20-slim

WORKDIR /app

COPY package.json .

RUN apt-get update && apt-get upgrade -y && npm install && apt-get clean && rm -rf /var/lib/apt/lists/*

COPY . .

EXPOSE 3000

CMD [ "node", "app.mjs" ]