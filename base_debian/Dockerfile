FROM debian:jessie
MAINTAINER Dave Potts <dave@goopot.co.uk>
RUN apt-get update
RUN apt-get install -y aptitude
RUN aptitude update
RUN aptitude --assume-yes safe-upgrade
RUN echo "Europe/London" > /etc/timezone
RUN dpkg-reconfigure --frontend noninteractive tzdata
RUN aptitude --assume-yes install git apt-utils ncdu ntp wget

