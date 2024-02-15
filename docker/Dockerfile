FROM node:alpine3.19

WORKDIR /usr/app

COPY package.json ./

RUN npm install

COPY src/hello.js ./

EXPOSE 3000

CMD ["hello.js"]
