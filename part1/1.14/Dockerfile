FROM ruby:2.6.0

COPY rails-example-project /rails-example-project

RUN apt-get update && apt-get install -y nodejs

RUN gem install bundler
RUN cd rails-example-project/ && bundle install && rails db:migrate
WORKDIR /rails-example-project
CMD rails s
