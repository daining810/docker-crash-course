FROM node:16.20.2

WORKDIR /home/api

COPY ./package.json .

RUN npm i

COPY . .

EXPOSE 4000

CMD ["npm", "run", "dev"]