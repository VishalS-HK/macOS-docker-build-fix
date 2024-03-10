# macOS-docker-build-fix

To fix the "Error load metadata for docker.io "issue, run the following commands in the given order:

1. Remove the Docker config file:
```bash
rm ~/.docker/config.json
```

2. Next, we clear the Docker cache
```bash
sudo rm -rf ~/.docker/buildx
```

3.Log out of Docker
```bash
docker logout
```

4. Log back in!!
```bash
docker login
```
