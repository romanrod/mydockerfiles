FROM ruby:2.5.3
MAINTAINER Roman Rodriguez <roman.g.rodriguez@gmail.com>
RUN apt-get update
RUN apt-get install -y 	apt-transport-https
RUN apt-get install libmagickwand-dev

RUN gem install bundler

# Chrome.
RUN wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | apt-key add - 
RUN sh -c 'echo "deb https://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
RUN apt-get update
RUN apt-get install -y google-chrome-stable

# headless
RUN apt-get install -y xvfb
