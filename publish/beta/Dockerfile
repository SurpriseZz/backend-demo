FROM registry.cn-hangzhou.aliyuncs.com/library/node:18

RUN mkdir -p /app/elpis-demo
WORKDIR /app/elpis-demo

COPY . /app/elpis-demo

ENV TZ=Asia/Shanghai

EXPOSE 8081

ENTRYPOINT ["npm", "run", "beta"]
