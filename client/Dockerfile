FROM node:18-alpine

# Add the following lines
ENV CI=true
ENV WDS_SOCKET_PORT=0

WORKDIR /app/client

COPY ./package*.json .

RUN npm install

COPY . .

CMD ["npm", "run", "start"]