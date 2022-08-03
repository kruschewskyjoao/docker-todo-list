FROM mjgargani/puppeteer:trybe1.0 as build
WORKDIR /app
COPY package*.json ./
RUN npm install
ADD node_modules.tar.gz ./
COPY . .
CMD [ "npm", "test" ]