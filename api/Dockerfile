FROM node:14.15.5-alpine3.13
RUN apk add --no-cache bash git
RUN npm config set cache /api/.npm-cache --global]
WORKDIR /app
USER node
RUN npm install
COPY . .
EXPOSE 8080
CMD ["node", "app.js"]