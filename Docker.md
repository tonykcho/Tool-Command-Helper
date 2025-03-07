# This is a reference/summary of Docker command commonly used.

## docker run
```
docker run {docker_image_name}
```
options:
- -d: Detached mode, container run in the background.
- -p {local_port}:{container_port}: Port forwarding, map the current local port to the container port. Making the container public to the local machine. ``` docker run -p 8080:80 nginx:alpine```. Mapping local port 8080 to container port 80.
- -a: Attach to standard input/output, print the log/output in the local machine.
- -e {variable=value}: Set environment variable for the container.
- -rm: Delete the container when the container is closed/terminated/exited.
- -v {docker_volume_name}: Set the storage for the container.
- -name {custom_name}: Set the name for the container.

Common Usage:
1. Create and run container in background with port forwarding
    ```docker run -d -p 5000:80 {image_name}```
2. Create and run a named container with volume mounted
    ```docker run -name {name} -v {volume_name}```
    
## docker exec
```
docker exec {container_id} {command}
```
options:
- -i: Interactive mode, allow standard input.
- -t: Allocate pseudo-tty

Common Usage:
1. Access Shell in the container
    ```docker exec -it {container_id} sh```
