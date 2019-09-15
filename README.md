# orihttp
check your original http request

# run
```bash
go run main.go
```

# build
```bash
go build -o orihttp main.go
```

# flag
```
-addr address server listen address eg: ":80" or "0.0.0.0:8080" default "127.0.0.1:9300"
```

# demo
地址： [ori.codetech.top](https://ori.codetech.top)

此demo因为使用apache反向代理，所以返回的请求头中有三个额外的`X-Forwarded-`参数，以及当发送的请求头中未设置Host时会得到`Host: 127.0.0.1:9001`。使用[ori.codetech.top:9001](http://ori.codetech.top:9001/)可以得到准确的原始http请求。
