FROM nginx:1.27

# Installer git (Debian-based image)
RUN apt-get update && apt-get install -y git

WORKDIR /usr/share/nginx/html

# Clone ton repository frontend
RUN git clone https://github.com/LoganPal/eval-docker-logan.git .

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
