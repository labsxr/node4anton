## Node.js guideline
https://cheatsheetseries.owasp.org/cheatsheets/NodeJS_Docker_Cheat_Sheet.html

### build
build for arm
```
docker buildx build --progress=plain --no-cache --platform linux/arm64 \
        --file ./docker/Dockerfile \
        --tag node4anton:0.1.0 .
```
build for x86
```
docker buildx build --progress=plain --no-cache --platform linux/amd64 \
        --file ./docker/Dockerfile \
        --tag node4anton:0.1.0 .
```
### run
```
docker run -p 3000:3000 node4anton:0.1.0
```
