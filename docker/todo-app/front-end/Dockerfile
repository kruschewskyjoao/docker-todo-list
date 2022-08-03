FROM node:14-alpine as build
WORKDIR /app
COPY package*.json ./
RUN npm install
ADD node_modules.tar.gz ./
COPY . .
EXPOSE 3000
CMD [ "npm", "start" ]