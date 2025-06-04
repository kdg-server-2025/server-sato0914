FROM golang:alpine
WORKDIR /app
COPY main.go .
RUN go build -o hello main.go
CMD ["./hello"]