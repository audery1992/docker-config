FROM golang
RUN apt-get update && apt-get install -y vim
RUN go get github.com/astaxie/beego && go get github.com/beego/bee

EXPOSE 8091

CMD ["bee","run"]
