FROM node:18-alpine

WORKDIR /app

COPY ./package.json ./
COPY ./package-lock.json ./

COPY ./index.js ./

RUN npm install

CMD ["npm", "start"]