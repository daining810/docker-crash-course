FROM node:17-alpine

# 安装node监听器,监听js和json文件的变化,立即响应
RUN npm install -g nodemon

# 一定要注意工作路径，在 compose 的时候挂在的卷是相关的
WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 4000

CMD ["npm", "run", "dev"]

