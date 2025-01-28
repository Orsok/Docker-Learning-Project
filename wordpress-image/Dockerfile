FROM ubuntu:18.04
LABEL maintainer="julianandrei.tcaciuc@de.ebmpapst.com"
RUN  apt-get -y update && apt-get -y install wordpress
COPY files/default /etc/nginx/sites-available/default
COPY files/index.html /usr/share/nginx/html/index.html
EXPOSE 80
CMD ["/usr/sbin/nginx", "-g", "daemon off;"]

