# image to use
FROM ubuntu:18.04

#Image build by
MAINTAINER 21050832@rp.edu.sg

#Install Apache2 package
RUN apt-get update
RUN apt-get install -y apt-utils
RUN apt-get install -y apache2
RUN apt-get install -y apache2-utils
RUN apt-get clean

# creat web volume
RUN mkdir myweb
COPY index.html /var/www/html/
VOLUME /myweb

CMD ["service apache2 restart", "-D", "FOREGROUND"]
CMD ["/bin/bash"]
# published on port 80
EXPOSE 80
