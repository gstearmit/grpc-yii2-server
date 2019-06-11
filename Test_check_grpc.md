##----------------Call test grpc boxme-----------------------
https://njp.io/grpcc-a-simple-command-line-client-for-grpc-services/

$ npm install -g grpcc
$ grpcc --proto Greeter.proto --address 127.0.0.1:50051 -i

Connecting to greeter.Greeter on 127.0.0.1:50051. Available globals:

  client - the client connection to Greeter
    sayHello (SayHelloRequest, callback) returns SayHelloResponse
    sayDebug (SayDebugRequest, callback) returns SayDebugResponse
    sayRepeated (SayRepeatedRequest, callback) returns SayRepeatedResponse

  printReply - function to easily print a unary call reply (alias: pr)
  streamReply - function to easily print stream call replies (alias: sr)
  createMetadata - convert JS objects into grpc metadata instances (alias: cm)
  printMetadata - function to easily print a unary call's metadata (alias: pm)

Greeter@127.0.0.1:50051> (node:21332) DeprecationWarning: grpc.load: Use the @grpc/proto-loader module with grpc.loadPackageDefinition instead
