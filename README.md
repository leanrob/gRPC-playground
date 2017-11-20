# gRPC-playground
sRPC is super powerful for inter-service communications. This is a place to experiment with it it and see its power.

## Requirements

This project MUST be in the /src folder of your go installation to run go and the packages.

Install Protocol Buffers through HomeBrew...

`brew doctor && brew install protobuf`

Install proto-den-go with go get...

`go get -u github.com/golang/protobuf/{proto,protoc-gen-go}`


## Setting up Hello World (In Go and Nodejs)

Create folder structure and proto file with the following string of commands...

`mkdir go && mkdir nodejs && mkdir pb && mkdir go/src && touch pb/messages.proto`

Then create the protocol code in golang using the following command...

`protoc pb/messages.proto --go_out=plugins=grpc:go/src`

