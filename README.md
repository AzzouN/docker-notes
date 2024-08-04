# Docker

## Notes

- A container is not supposed to stay alive forever, the container is supposed to run a specific task or process and stays alive as long as the process is alive and exist as soon as the process or task finish.
- When we start create a container from image using the run command we can specify the command that we want to execute.
- When we run a container from an image, we will be in attached mode by default, to run a container in detached mode we cann pass **-d** argument to **docker run** command, and we can attach to our container later using **docker attach**.

## Commands

```bash
# Creates a container from a docker image, if the image does not exist on the host OS, it will be fetched from docker-hub
docker run <image_name> 
```

```bash
# List containers
docker ps
```

```bash
# Stop a running container
docker stop <container_name or container_id>
```

```bash
# Start a stopped container
docker start <container_name or container_id>
```

```bash
# Delete a container
docker rm <container_name or container_id>
```

```bash
# List the images that we have in the host OS
docker images
```

```bash
# Delete a docker image
docker rmi <image_name>
```

```bash
# Pull an image from docker-hub without creating a container
docker pull
```

```bash
# Execute a specific command when creating the container from the image
docker run ubuntu <command> <command_args>
```

```bash
# Execute a command in a running container
docker exec <container_name or container_id> <command> <command_args>
```

```bash
# Run a container in detached mode
docker run -d ubuntu
```

```bash
# Attach to a container
docker attach <container_name or container_id>
```

```bash
```

```bash
```
