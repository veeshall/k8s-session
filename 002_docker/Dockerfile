FROM golang:1.8

WORKDIR /go/src/app
COPY hello.go .

RUN go get -d -v ./...
RUN go install -v ./...

EXPOSE 80
CMD ["app"]
