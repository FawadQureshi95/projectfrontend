FROM node:10-alpine

LABEL name="Node Express Application" \   
     maintainer="Fawad Tariq <fawadqureshi1995@gmail.com>" \
     summary="A Node Express application"

# Create app directory
WORKDIR /app

EXPOSE 8080

COPY frontend-node/package*.json ./

RUN npm install

RUN apk add curl 

COPY frontend-node/server.js ./

CMD [ "npm", "start" ]
