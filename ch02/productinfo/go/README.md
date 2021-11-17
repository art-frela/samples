# ``ProductInfo`` Service and Client - Go Implementation

## Building and Running Service

In order to build, Go to ``Go`` module root directory location (productinfo/go/server) and execute the following
 shell command,

```bash
go build -v -o bin/server
```

In order to run, Go to ``Go`` module root directory location (productinfo/go/server) and execute the following
shell command,

```bash
./bin/server
```

## Building and Running Client  

In order to build, Go to ``Go`` module root directory location (productinfo/go/client) and execute the following
 shell command,

```bash
go build -v -o bin/client
```

In order to run, Go to ``Go`` module root directory location (productinfo/go/client) and execute the following
shell command,

```bash
./bin/client
```

## Additional Information

### Generate Server and Client side code

[protocol-buffers/docs/reference/go-generated](https://developers.google.com/protocol-buffers/docs/reference/go-generated#package)

Pre-generated stub file is included in the go project. If you need to generate the stub files please use the below
 command from the root directory(inside productinfo directory)

```bash
protoc --go_out=go/server/ecommerce \
    --go-grpc_out=go/server/ecommerce \
    proto/product_info.proto

protoc --go_out=go/client/ecommerce \
    --go-grpc_out=go/client/ecommerce \
    proto/product_info.proto
```
