# Using google-protobuf

```bash
./node_modules/.bin/grpc_tools_node_protoc \
  --plugin=protoc-gen-ts=./node_modules/.bin/protoc-gen-ts \
  --js_out=import_style=commonjs,binary:./src/compiled_proto \
  --ts_out=service=grpc-web:./src/compiled_proto \
  --proto_path=./proto_origin \
  ./proto_origin/items.proto
```