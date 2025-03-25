FROM nginx:1.27
RUN apk add --no-cache git
WORKDIR /usr/share/nginx/html
COPY index.html .
RUN git clone https://github.com/LoganPal/eval-docker-logan .
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
