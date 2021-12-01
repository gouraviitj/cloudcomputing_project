FROM kapacitor
RUN apt-get update
RUN apt-get install python-pip3 -y
RUN docker images -y
RUN docker pull kapacitor
RUN docker images -y
RUN docker container ls -y
RUN docker run kapacitor
RUN docker container ls -y