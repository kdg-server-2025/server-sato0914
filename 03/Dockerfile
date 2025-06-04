FROM golang:alpine
#goの設定されたalpine

WORKDIR /
COPY main.go .
#main.goを.のコンテナにコピー
RUN go build main.go

CMD ["./main"]