## Login Docker to Github registry
```echo YOUR_GITHUB_TOKEN | docker login ghcr.io -u YOUR_GITHUB_USERNAME --password-stdin```

## Pushing docker image to Github Registry
docker tag my-image ghcr.io/USERNAME/my-image:latest
docker push ghcr.io/USERNAME/my-image:latest

