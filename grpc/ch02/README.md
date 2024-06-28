# Ch02

```
protoc -I proto/ proto/product_info.proto --go_out=plugins=grpc:server/ecommerce
protoc -I proto/ proto/product_info.proto --go_out=plugins=grpc:client/ecommerce

mkdir build
cd server && go build -v -o ../build/server && cd ..
cd client && go build -v -o ../build/client && cd ..

./build/server
./build/client
```

