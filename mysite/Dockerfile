FROM ubuntu:latest
RUN apt-get update
RUN apt-get install -y nginx
COPY ./testsite.conf /etc/nginx/sites-enabled/testsite.local.conf
WORKDIR /var/www
VOLUME /home/mysyte/www
EXPOSE 8080
CMD ["nginx", "-g", "daemon off;"]
