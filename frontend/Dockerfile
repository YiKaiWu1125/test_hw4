# 使用 Node.js 作為基礎映像
FROM docker.io/library/node:21-alpine3.18 AS RUNNER

# 設定工作目錄
WORKDIR /frontend

# 複製所有程式碼到容器中
COPY ./ ./

# 安裝相依套件
RUN npm install

# 設定容器的對外口
EXPOSE 5173

# 啟動開發模式
CMD ["npm", "run", "dev"]
