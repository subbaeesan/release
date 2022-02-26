# image to use
FROM ubuntu:18.04

#Image build by
MAINTAINER 21050832@rp.edu.sg

#Install Apache2 package
RUN apt-get update && \
apt-get install -y apache2 && \
apt clean

# Copy web pages
ADD Planet-Crops.tar.xz /var/www/
COPY /var/www/Planet-Crops/ /var/www/html/

CMD ["/usr/sbin/apache2ctl start", "-D", "FOREGROUND"]
CMD ["/bin/bash"]
# published on port 80
EXPOSE 80
