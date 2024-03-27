FROM node:17-alpine

# 安装node监听器,监听js和json文件的变化,立即响应
RUN npm install -g nodemon

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 4000

CMD ["npm", "run", "dev"]

