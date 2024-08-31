FROM node:12
WORKDIR /app

ENV NODE_ENV=production

COPY package*json ./

RUN npm install

COPY . .

RUN npm install -g pm2

EXPOSE 3001

CMD ["pm2-runtime", "index.js"]
