FROM ruby:2.3

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app/
ADD . /usr/src/app

RUN bundle install

# Cleanup
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /var/tmp/* /tmp/*
RUN rm -rf /usr/src/app/tmp