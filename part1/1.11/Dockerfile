FROM ubuntu

RUN apt-get update && apt-get install -y curl wget
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs
COPY backend-example-docker /backend-example-docker
EXPOSE 8000
RUN cd backend-example-docker/ && npm install

WORKDIR /backend-example-docker

CMD ["npm", "start"]
