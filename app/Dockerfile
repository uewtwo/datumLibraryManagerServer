FROM golang:1.13

ENV GOPATH /go
ENV PATH $PATH:$GOPATH/bin

RUN mkdir -p /go/app
WORKDIR /go/app
ENV GO111MODULE=on

COPY . .

RUN go get github.com/labstack/echo \
      github.com/oxequa/realize \
  && go build -o app

