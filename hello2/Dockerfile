FROM ubuntu:22.04
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y figlet
COPY ./hello.sh /hello.sh
ENTRYPOINT [ "/hello.sh" ]
