FROM golang:1.13

ENV GOPATH /go
ENV PATH $PATH:$GOPATH/bin

RUN mkdir -p /go/app
WORKDIR /go/app

COPY . .

RUN set -ex && \
  go get github.com/labstack/echo && \
  go get github.com/oxequa/realize && \
  go build -o app

