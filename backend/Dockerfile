FROM node:20

RUN apt-get update && apt-get install -y git

WORKDIR /app

RUN git clone https://github.com/LoganPal/eval-docker-logan.git . && \
    cp -r backend/* . && \
    rm -rf backend

RUN npm install

EXPOSE 3000

CMD ["node", "server.js"]