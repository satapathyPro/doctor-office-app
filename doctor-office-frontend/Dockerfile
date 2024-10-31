FROM node:20.8.0
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
EXPOSE 3001
CMD ["npx", "serve", "-s", "build", "-l", "3001"]
