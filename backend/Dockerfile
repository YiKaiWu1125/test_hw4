# 使用 Node.js 作為基礎映像
FROM docker.io/library/node:21-alpine3.18 AS RUNNER

# 設定工作目錄
WORKDIR /backend

# 複製所有程式碼到容器中
COPY ./ ./
COPY .env.sample .env

# 設定容器的對外口
EXPOSE 8888

# 安裝應用程式的相依套件
RUN npm install

# 啟動應用程式的開發模式
CMD ["npm", "run", "dev"]
