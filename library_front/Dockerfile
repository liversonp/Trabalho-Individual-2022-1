FROM node:16.17.0

WORKDIR /library_front

COPY package*.json ./

COPY package-lock.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm","start"]