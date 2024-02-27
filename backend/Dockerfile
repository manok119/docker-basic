# node.js 이미지를 바탕으로 컨테이너를 실행한 후
# http://localhost:3333으로 접속했을 때 hello from server 메시지가 표시되게 만드세요

# /backend/Dockerfile
FROM node:16-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy the package.json file and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the code
COPY . .

# The application is set to listen on port 80, expose it
EXPOSE 80

# Start the application
CMD ["node", "app.js"]