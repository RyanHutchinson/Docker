FROM ruby:2.2.0
RUN mkdir /app
WORKDIR /app
ADD . /app
RUN bundle install
CMD bundle exec puma config.ru -p $PORT -e production

# git clone https://github.com/devigned/docker-ruby-hello-world.git hello_world
# export PORT=8080
# docker build -t ruby-sample .
# ID=$(docker run -e "PORT=$PORT" -p $PORT:$PORT -d ruby-sample)
# open this in browser -----> "http://localhost:8080"