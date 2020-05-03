### Code Snippets

Generate the `.pb.go` files using `protoc`
```bash
protoc -I proto proto/ProductInfo.proto --go_out=plugins=grpc:$(pwd)/service/ecommerce
protoc -I proto proto/ProductInfo.proto --go_out=plugins=grpc:$(pwd)/client/ecommerce
```

Run the server, then the client
```bash
service/bin/server
client/bin/client
```
