FROM ubuntu
RUN apt-get update && apt-get install -y locales && rm -rf /var/lib/apt/lists/* \
    && localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
ENV LANG en_US.utf8


COPY Server.rar /.
RUN apt-get install -y unzip
RUN unzip Server.rar
RUN chmod +x /Server.x86_64
CMD /Server.x86_64
