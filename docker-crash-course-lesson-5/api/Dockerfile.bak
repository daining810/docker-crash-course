# 定义父镜像
FROM node:17-alpine

# 定义工作目录为容器根目录下的/app
# 一旦指定了工作目录则接下来所有的操作都是相对于该目录
WORKDIR /app

# 从Dockerfile所在的目录拷贝所有文件到WORKDIR指定的目录中
# 第一个.是相对于Dockerfile所在的目录
# 第二个.是相对于WORKDIR所在的目录
COPY . .

# 安装依赖
RUN npm install

# 显示指定暴露的端口,这里有注释的成分,让人一目了然所要暴露的端口,运行容器的时候也可以通过参数指定端口映射
# 这里的定义还会显示在Docker Desktop上,运行镜像是,填写端口映射会出现
EXPOSE 4000

# 在容器中运行镜像,注意RUN是用来构建镜像的指令,CMD是运行镜像的指令
CMD ["node", "app.js"]

