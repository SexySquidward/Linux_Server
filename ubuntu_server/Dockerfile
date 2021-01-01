FROM ubuntu
RUN \
    sed -i 's/# \(.*multiverse$\)/\1/g' /etc/apt/sources.list && \
    apt-get update && \
    apt-get -y upgrade && \
    apt-get install -y unrar && \
    apt-get install -y build-essential && \
    apt-get install -y software-properties-common && \
    apt-get install -y byobu curl git htop man unzip vim wget && \
    rm -rf /var/lib/apt/lists/*


COPY Server.rar /etc/Server
RUN unrar x Server.rar
RUN chmod +x /Server.x86_64
CMD ["bash"]

