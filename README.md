# kb-api

Kilobook api

# install

## install plugins

`# vendor/bin/extas i`

## generate api specs

`# vendor/bin/extas jsonrpc -s extas.json`

## install specs

`# vendor/bin/extas i`

# usage

## set EXTAS__BASE_PATH

`# export EXTAS__BASE_PATH=/your/path`

## run server

`# php -S 0.0.0.0:8080 -t vendor/jeyroik/extas-jsonrpc/src/public`

## check specs

`curl -X POST localhost:8080/specs -d "{\"id\":\"request id\", \"method\":\"operation.all\"}"`

## use api

Warning: fill the data before using

`curl -X POST localhost:8080/api/jsonrpc -d "{\"id\":\"request id\", \"method\":\"book.create\", \"data\":{...}}"`
