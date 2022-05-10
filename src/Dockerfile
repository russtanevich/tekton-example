FROM golang:1.16-alpine

RUN apt install libgeos librdkafka

WORKDIR /go/src/app
COPY . .

RUN go install -v ./...

CMD ["app"]
