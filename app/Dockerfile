# syntax=docker/dockerfile:1

FROM node:12.18.1
ENV NODE_ENV=production

WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]

RUN npm install --production --platform linux/amd64

COPY . .

EXPOSE 8080
CMD [ "node", "server.js" ]
