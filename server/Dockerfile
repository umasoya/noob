FROM golang:alpine

RUN apk --no-cache add git go && \
        go get -v github.com/magefile/mage && \
        go get -d -v github.com/gohugoio/hugo && \
        cd ${GOPATH}/src/github.com/gohugoio/hugo && \
        mage -v vendor && \
        mage -v install
