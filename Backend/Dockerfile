FROM golang:1.22-alpine

WORKDIR /app

COPY go.mod ./
# REMOVE or COMMENT the next line
# COPY go.sum ./

RUN go mod download

COPY main.go ./

RUN go build -o server .

CMD ["./server"]

EXPOSE 8080

