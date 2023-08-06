# Docker Build and Push Action

This GitHub action constructs a full Docker image reference using the provided inputs, then builds and pushes the Docker image to the specified Docker repository.

## Inputs

### `docker_repo_hostname`

**Required** Hostname of the Docker repository.

### `container_image_repo`

**Required** Repo of the Docker image to be built and pushed.

### `container_image_tag`

**Required** Tag of the Docker image to be built and pushed.

## Usage

```yaml
steps:
  - name: Docker Build and Push
    uses: plantoncloud/docker-build-and-push-action@main
    with:
      docker_repo_hostname: your-docker-repo-hostname
      container_image_repo: your-image-repo-name
      container_image_tag: your-image-tag
```

Upon completion of this action, the Docker image specified by the `container_image_repo` and `container_image_tag` inputs will be built and pushed to the repository denoted by `docker_repo_hostname`.

## Contributing

If you have suggestions for how this GitHub Action could be improved, or want to report a bug, open an issue! We'd love all and any contributions.

## License

This project is licensed under the [MIT License](LICENSE).
