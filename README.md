# hello-app
When compiling image:
- if buildx is not enable:
```
docker buildx create --use
```
Build image and push to Docker Hub (arm/x86):
```
docker buildx build --platform linux/amd64,linux/arm64 -t arthuracrs/hello . --push
```
```
kubectl set image deployment/hello-deployment hello-container=arthuracrs/hello:1.0.2
```
