FROM debian

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y cowsay fortune lolcat

ENTRYPOINT /usr/games/fortune | /usr/games/cowsay | /usr/games/lolcat

#build with: docker build -t bonus02 .
#run with:   docker run -it bonus 02
