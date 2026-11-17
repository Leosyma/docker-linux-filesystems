# Linux filesystems in Docker

The walkthrough in LEIAME.txt compares bind mounts with Docker volumes. Write files inside an Ubuntu container and attach its storage to another container to see which changes persist. Substitute your own host directory for the example path.

## Run locally

```sh
docker volume create lab-data
docker run --rm -it -v lab-data:/data ubuntu bash
```
