FROM node:12
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# package.json and package-lock.json

COPY package*.json ./
COPY .env ./
RUN npm install
COPY . .
EXPOSE 5000
CMD ["npm", "run", "search"]