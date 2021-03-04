FROM node:14.15.5-alpine3.13
RUN apk add --no-cache bash git
WORKDIR /app
COPY package*.json ./
RUN npm install
USER node
COPY . .
EXPOSE 8080
CMD ["node", "src/app.js"]