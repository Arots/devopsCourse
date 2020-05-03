FROM ubuntu

RUN apt-get update && apt-get install -y curl wget && curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs

COPY frontend-example-docker /frontend-example-docker
#RUN chmod a+rx /frontend-example-docker
EXPOSE 5000
RUN cd frontend-example-docker/ && npm install

WORKDIR /frontend-example-docker

CMD ["npm", "start"]

#RUN npm install
#RUN npm install -g serve
#RUN npm start
