FROM base

RUN apt-get update
RUN apt-get -y install build-essential git libssl-dev curl

RUN git clone https://github.com/sstephenson/rbenv.git /usr/local/rbenv

RUN mkdir /usr/local/rbenv/plugins
RUN git clone https://github.com/sstephenson/ruby-build.git /usr/local/rbenv/plugins/ruby-build

ENV RBENV_ROOT /usr/local/rbenv

ENV PATH /usr/local/rbenv/shims:/usr/local/rbenv/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin

RUN rbenv install 2.0.0-p247

ENV RBENV_VERSION 2.0.0-p247

RUN gem install bundler
