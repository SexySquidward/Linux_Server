FROM ubuntu
RUN \
    apt-get update && \
    apt-get -y upgrade && \
    apt-get install -y unzip


COPY Server.rar /etc/Server
RUN unzip Server.rar
RUN chmod +x /Server.x86_64
CMD /Server.x86_64

