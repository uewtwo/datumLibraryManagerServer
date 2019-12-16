FROM golang:1.13

ENV GOPATH /go
ENV PATH $PATH:$GOPATH/bin
ENV GOM111MODULE=on

RUN mkdir -p /go/src/datum-library-manager-server
WORKDIR /go/src/datum-library-manager-server

COPY . .

RUN set -ex && \
  go get gopkg.in/urfave/cli.v2@master && \
  go get github.com/oxequa/realize && \
  go mod download

