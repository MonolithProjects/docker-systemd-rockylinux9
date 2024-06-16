# Rocky Linux 9 Ansible Test Image

[![Publish Image](https://github.com/MonolithProjects/docker-systemd-rockylinux9/actions/workflows/publish.yml/badge.svg)](https://github.com/MonolithProjects/docker-systemd-rockylinux9/actions/workflows/publish.yml)
[![DockerHub-pulls](https://img.shields.io/docker/pulls/monolithprojects/systemd-rockylinux9)](https://hub.docker.com/repository/docker/monolithprojects/systemd-rockylinux9)
[![DockerHub](https://img.shields.io/docker/image-size/monolithprojects/systemd-rockylinux9)](https://hub.docker.com/repository/docker/monolithprojects/systemd-rockylinux9)

Docker image with rockylinux9 and enabled systemd. Image is updated with the latest software updates on the 1st day in the month. Image contains also `ansible` user (UID/GID 1000) with NOPASSWD:ALL sudo rights.  

**Note:** This docker image is ment to be used for Molecule Ansible tests and development purpose. I do not recomend to use it in production.

## Tags

- `latest`  
- `<monthly build timestamp>` for the list of the tags see the [Docker Hub](https://hub.docker.com/repository/docker/monolithprojects/systemd-rockylinux9/tags?page=1)

## How-to

  1. Pull image with command `docker pull monolithprojects/systemd-rockylinux9:latest`  
  2. Run the container from the image: `docker run --detach --privileged --volume=/sys/fs/cgroup:/sys/fs/cgroup:ro monolithprojects/systemd-rockylinux9:latest`  

## License

MIT
