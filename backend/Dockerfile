FROM golang:1.15.2-alpine3.12

COPY . /go/src/api

WORKDIR /go/src/api

RUN apk update \
  && apk add --no-cache git \
  && go get github.com/gin-gonic/gin \
  && go get github.com/jinzhu/gorm \
  && go get github.com/go-sql-driver/mysql \
  && go get github.com/pilu/fresh

EXPOSE 8080

CMD ["fresh"]
