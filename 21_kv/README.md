# example

## server

```console
   Compiling kv v0.1.1 (/lyndon/iProject/rustpath/src/github.com/geektime-rust/21_kv)
    Finished dev [unoptimized + debuginfo] target(s) in 27.64s
     Running `target/debug/examples/server`
2022-06-20T12:11:31.418198Z  INFO server: Start listening on 127.0.0.1:9527
2022-06-20T12:12:10.365360Z  INFO server: Client 127.0.0.1:50214 connected
2022-06-20T12:12:10.365538Z  INFO server: Got a new command: CommandRequest { request_data: Some(Hset(Hset { table: "table1", pair: Some(Kvpair { key: "hello", value: Some(Value { value: Some(String("world")) }) }) })) }
2022-06-20T12:12:10.366018Z  INFO server: Client 127.0.0.1:50214 disconnected
```


## client
```console
   Compiling kv v0.1.1 (/lyndon/iProject/rustpath/src/github.com/geektime-rust/21_kv)
    Finished dev [unoptimized + debuginfo] target(s) in 1.38s
     Running `target/debug/examples/client`
2022-06-20T12:12:10.365866Z  INFO client: Got response CommandResponse { status: 200, message: "", values: [Value { value: None }], pairs: [] }
```