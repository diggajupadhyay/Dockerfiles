FROM golang:1.18.2-alpine

WORKDIR /usr/src/typioca

COPY go.mod go.sum ./
RUN go mod download && go mod verify

COPY . .
RUN go build -v -o /usr/local/bin/typioca ./...

CMD [ "typioca" ]
