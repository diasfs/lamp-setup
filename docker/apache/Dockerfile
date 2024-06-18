FROM debian:sid-slim
RUN apt update && apt install -y --no-install-recommends apache2
RUN a2enmod rewrite
RUN a2enmod proxy_fcgi
RUN a2enmod headers
RUN a2enmod actions
CMD ["/bin/sh", "-c", "/usr/sbin/apache2ctl -D FOREGROUND"]
