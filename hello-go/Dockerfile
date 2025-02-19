FROM golang:1.21.3 AS dev
COPY . /root/hello-go/
RUN go build -o /hello-go /root/hello-go/hello.go
FROM scratch
COPY --from=dev /hello-go .
ENTRYPOINT [ "/hello-go" ]
