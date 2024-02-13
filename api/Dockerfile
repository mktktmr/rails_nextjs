FROM ruby:3.2.3-slim
RUN apt-get update -qq && apt-get install -y build-essential default-libmysqlclient-dev
RUN mkdir /app
WORKDIR /app
ADD Gemfile /app/Gemfile
ADD Gemfile.lock /myapp/Gemfile.lock
RUN bundle install
ADD . /app
