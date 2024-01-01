## Build the image for a new architecture

```bash
docker build --tag fpultar/actions-image-armv8:latest --build-arg RUNNER_VERSION=2.311.0 --build-arg ARCHITECTURE=arm64 .
docker push fpultar/actions-image-armv8:latest
```

## Start the runner

** Don't forget to change the image name in `compose.yml` **

```bash
export REPO=...
export TOKEN=...
docker compose up
```
