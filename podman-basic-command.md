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

1.3 Running Containers with Podman

The podman run command allows you to start a new container from an image. Here are some options you might use:

```bash
podman run -d -p 8080:80 --name my-web-server nginx
```

Explanation:

    -d: Runs the container in detached mode (in the background).
    -p 8080:80: Maps port 80 in the container to port 8080 on the host.
    --name my-web-server: Assigns the container a custom name.

To list all running containers:

```bash
podman ps
```

To list all containers, including stopped ones:

```bash
podman ps -a
```

