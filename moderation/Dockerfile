FROM node:18-alpine

WORKDIR /app/post

COPY ./package.json .

RUN npm install

COPY . .

CMD ["node", "index.js"]