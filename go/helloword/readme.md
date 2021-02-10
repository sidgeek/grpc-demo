
1、 write the proto file to define the rpc function

2、 make go proto function define with protoc
protoc --go_out=. --go_opt=paths=source_relative \
    --go-grpc_out=. --go-grpc_opt=paths=source_relative \
    protos/helloword.proto


protoc --proto_path=proto proto/*.proto --go_out=plugins=grpc:pb


will make 2 files:
    helloword_grpc.pb.go
    helloword.pb.go


3、Implete the server


