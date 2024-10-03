FROM node:22-alpine

WORKDIR /usr/src/app

COPY . /usr/src/app/

RUN npm init -y

RUN npm install express

EXPOSE 3000

CMD [ "node", "index.js" ]