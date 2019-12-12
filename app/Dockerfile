FROM golang:1.13

ENV GOPATH /go
ENV PATH $PATH:$GOPATH/bin

RUN mkdir -p /go/app
COPY . /go/app
WORKDIR /go/app

RUN go get github.com/labstack/echo

