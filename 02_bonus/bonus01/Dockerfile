FROM debian

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y \
		git \
		make \
		gcc 
		
RUN git clone https://github.com/klange/nyancat.git

WORKDIR nyancat

RUN make && cd src

CMD ./src/nyancat

# docker build -t nyancat
# docker run -it nyancat	
