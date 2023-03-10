FROM ubuntu:latest
RUN apt update
RUN apt install cowsay -y
ENV PATH=$PATH:/usr/games
RUN cowsay "Holaaa desde docker"

RUN apt install apache2 -y
#RUN service apache2 start

COPY index.html ./var/www/html/

CMD ["apache2ctl", "-D", "FOREGROUND"]

EXPOSE 80

#CMD /bin/bash
