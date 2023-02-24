# hello-app
When compiling image:
- if buildx is not enable:
```
docker buildx create --use
```
Build image (arm/x86):
```
docker buildx build --platform linux/amd64,linux/arm64 -t arthuracrs/hello .
```

After all Push to Docker Hub
```
docker push arthuracrs/hello
```
