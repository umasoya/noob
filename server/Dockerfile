FROM golang:alpine

RUN apk --no-cache add git go && \
        go get github.com/kardianos/govendor && \
        govendor get github.com/gohugoio/hugo && \
        go install github.com/gohugoio/hugo
