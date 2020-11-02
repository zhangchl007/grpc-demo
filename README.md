# grpc-demo

1. Prepare for the env

```
go get -u google.golang.org/grpc

brew install protobuf

go get -u github.com/golang/protobuf/protoc-gen-go

```

2. Compiling The Protobuf Definition

```
protoc -I pkg/proto/credit/ pkg/proto/credit/credit.proto --go_out=plugins=grpc:pkg/proto/credit/

```
3. Deploy server and client

```
make server

make client
```
Reference: http://www.inanzzz.com
