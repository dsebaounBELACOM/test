FROM debian:latest
RUN apt-get update
RUN apt-get --assume-yes install default-jdk
RUN mkdir /opt/sparkJobs
COPY ./projects /opt/sparkJobs
EXPOSE 6066 7077 7078 8080 8081
RUN echo "deb https://dl.bintray.com/sbt/debian /" | tee -a /etc/apt/sources.list.d/sbt.list
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 2EE0EA64E40A89B84B2DF73499E82A75642AC823
RUN apt-get update
RUN apt-get --assume-yes install sbt
