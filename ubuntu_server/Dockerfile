FROM ubuntu
COPY Server.rar /.
RUN sudo apt install unzip
RUN unzip Server.rar
RUN chmod +x /Server.x86_64
CMD /Server.x86_64
