FROM docker.1ms.run/node:18
WORKDIR /app/elpis-demo

# 安装依赖
COPY package*.json ./
RUN npm install

# 复制源代码
COPY . /app/elpis-demo

# 打包
RUN npm run build:prod

ENV TZ=Asia/Shanghai
ENV _ENV=production
ENV PORT=8081

EXPOSE 8081

# 启动服务
CMD ["node", "./server.js"]