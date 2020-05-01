# hello-go
hello-go

# 打包镜像
```shell
CGO_ENABLED=0 GOOS=linux go build -a -installsuffix cgo -o hello-go .
docker build -t ganodermaking/hello-go:latest .
docker tag ganodermaking/hello-go:latest ganodermaking/hello-go:latest
docker push ganodermaking/hello-go:latest
```
