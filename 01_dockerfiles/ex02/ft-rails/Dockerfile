FROM ruby:2.4.1

RUN apt-get update -y && apt-get upgrade -y

RUN apt-get install -y \
			 node.js \
			 sqlite3 

ONBUILD EXPOSE 3000


ONBUILD WORKDIR /opt/app
ONBUILD COPY app /opt/app

ONBUILD RUN bundle install

ONBUILD RUN rake db:migrate
ONBUILD RUN rake db:seed
