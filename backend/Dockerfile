FROM golang:1.15.2-alpine

RUN apk update && apk add git

COPY /api/src /app/src

WORKDIR /app/src

# RUN go build -o main .
RUN go build -o main

ENV GO111MODULE=on

EXPOSE 8080
# CMD ["go", "run", "main.go"]
CMD [ "./main" ]