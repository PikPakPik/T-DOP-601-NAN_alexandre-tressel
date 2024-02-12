FROM node:12-alpine

ADD . /app/
WORKDIR /app
RUN npm install

COPY . .

EXPOSE 80


CMD [ "node", "server.js" ]