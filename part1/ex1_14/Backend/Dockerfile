FROM golang:1.16
EXPOSE 8080

WORKDIR /go/src/app
COPY . .

ENV REQUEST_ORIGIN=http://localhost:5000
ENV REDIS_HOST=redis_cache

RUN go build .

CMD ["./server"]
