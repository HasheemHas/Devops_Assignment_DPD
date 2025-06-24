FROM golang:1.22-alpine
WORKDIR /app
COPY . .
RUN go build -o main .
RUN apk add --no-cache curl
EXPOSE 8001
CMD ["./main"]

