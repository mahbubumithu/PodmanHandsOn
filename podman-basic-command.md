### Podman Basic Commands

1.1 Pulling Images

The podman pull command downloads container images from a registry. By default, it pulls from Docker Hub.

```bash
podman pull ubuntu:latest
```

This command pulls the latest Ubuntu image. We can also specify other versions or repositories.

1.2 Listing Images

To see all images stored on your system, use:

```bash
podman images
```

This will display all locally available container images, showing their REPOSITORY, TAG, IMAGE ID, and SIZE.