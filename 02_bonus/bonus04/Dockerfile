FROM ubuntu

ENV TZ=Europe/Moscow

RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y \
		git \
		vim \
		default-jdk \
		default-jre 

#docker build -t bonus04 .
#docker run -it --rm bonus04
