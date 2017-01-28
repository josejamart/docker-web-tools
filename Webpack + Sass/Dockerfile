FROM node:7.4

RUN apt-get update -q &&\
	apt-get install -y build-essential &&\
	apt-get install -y ruby &&\
	gem install sass --source http://rubygems.org &&\
	npm install -g webpack

RUN mkdir /src

WORKDIR /src

EXPOSE 3000
EXPOSE 35729

CMD ["npm","start"]
