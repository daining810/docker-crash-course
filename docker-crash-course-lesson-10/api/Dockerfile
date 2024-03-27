FROM node:16.20.2

WORKDIR /home/api

RUN npm i -g nodemon

COPY package.json .

RUN npm i

COPY . .

EXPOSE 4000

CMD ["npm", "run", "dev"]
