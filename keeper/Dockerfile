FROM node:20-alpine

WORKDIR /app

COPY . .

RUN npm install

RUN npx tsc

EXPOSE 3000

CMD ["node", "dist/index.js"]
