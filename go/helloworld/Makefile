gen:
	protoc --go_out=. --go_opt=paths=source_relative \
    --go-grpc_out=. --go-grpc_opt=paths=source_relative \
    proto/helloworld.proto

clean:
	rm proto/*.go

run:
	go run server/main.go

run-c:
	go run client/main.go
