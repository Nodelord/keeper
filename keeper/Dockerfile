FROM node:20-alpine

RUN pwd
RUN ls -la /
RUN ls -R .

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

RUN npx tsc

EXPOSE 3000

CMD ["node", "dist/index.js"]
