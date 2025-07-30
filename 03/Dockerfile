FROM golang:1.22-alpine AS builder
WORKDIR /app
COPY main.go .
#main.goを.のコンテナにコピー
RUN go build -o main main.go

FROM alpine:3.20
WORKDIR /app
COPY --from=builder /app/main .

CMD ["./main"]