FROM golang:1.9

RUN go get -v -u github.com/golang/dep/cmd/dep && \
      go get -d -v github.com/prologic/pastebin && \
      cd $GOPATH/src/github.com/prologic/pastebin && \
      dep init -v

RUN go install -v github.com/prologic/pastebin

EXPOSE 8000
