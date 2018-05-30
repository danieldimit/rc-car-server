
## gRPC and building the protobuffers

There are two ways to build the modules for the python client :

1) Using the protocol buffer from python (for proto3 use python 2.7)

```bash
python -m grpc_tools.protoc -I protos/ --python_out=. --grpc_python_out=. protos/client.proto
```

2) Installing the protocol buffer : https://github.com/grpc/grpc/blob/master/INSTALL.md

### Defining the proto file

This is the guide for defining **proto3** files: https://developers.google.com/protocol-buffers/docs/proto3

This is an example of a **proto3** file: https://github.com/grpc/grpc/blob/v1.6.x/examples/protos/route_guide.proto 

### Using the generated modules

This is an example of creating client / server code : https://grpc.io/docs/tutorials/basic/python.html