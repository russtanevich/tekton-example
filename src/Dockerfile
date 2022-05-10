FROM ubuntu:22.04

RUN apt update

RUN apt install -y golang-go && go version

RUN apt install libgeos-dev

WORKDIR /go/src/app
COPY . .

RUN go install -v ./...

CMD ["app"]
