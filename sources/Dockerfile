from ubuntu:16.04
LABEL maintainer="manuelbacallado89@gmail.com"

RUN apt-get update && apt-get install -y apache2 && apt-get clean && rm -rf /var/lib/apt/lists/*

EXPOSE 80
ADD ["index.html","/var/www/html"]

ENTRYPOINT ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
