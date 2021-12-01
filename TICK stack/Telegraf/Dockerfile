FROM telegraf
RUN apt-get update
RUN apt-get install python-pip3 -y
RUN docker images -y
RUN docker pull telegraf
RUN docker images -y
RUN docker container ls -y
RUN docker run telegraf
RUN docker container ls -y