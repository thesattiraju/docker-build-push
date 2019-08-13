# Docker build and push

This repo contains a workflow file.

# Prerequisites

The workflow does docker login for you to push to your docker registry, so it expects 2 secrets to be added to your repository.

- `username`: docker registry username
- `password`: docker registry password

The default registry server it pushes to is `https://index.docker.io/v1/` if you want to push to a different registry, add `login-server: <your-login-server>` to the `docker login` step. 
