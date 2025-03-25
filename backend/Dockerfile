FROM node:22
RUN apk add --no-cache git
WORKDIR /app
COPY package.json package-lock.json ./
RUN git clone https://github.com/LoganPal/eval-docker-logan .
RUN npm install
COPY . .
EXPOSE 3000
CMD ["node", "server.js"]