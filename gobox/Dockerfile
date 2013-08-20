FROM base
MAINTAINER Michael Gorsuch <michael.gorsuch@gmail.com>

RUN apt-get update
RUN apt-get install -y curl 

RUN cd /usr/local && curl -O https://go.googlecode.com/files/go1.1.2.linux-amd64.tar.gz

RUN cd /usr/local && tar xzf go1.1.2.linux-amd64.tar.gz

RUN cd /usr/local && rm go1.1.2.linux-amd64.tar.gz

ENV GOROOT /usr/local/go

RUN mkdir /go

ENV GOPATH /go

ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/go/bin:/go/bin
