# Docker crash course

## Create an image

`docker build -t my-express-app`

## Run the image (create new container)

`docker run --name express-cli -p 4000:4000 -d my-express-app`

-p: publish to localhost port

-d: detach

## Start the container (existed)

`docker start express-cli (names)`

## Remove image (not in use)

`docker image rm myapp`

`docker image rm myapp -f` (force delete)

## Remove a container

`docker container rm container-name`

## Common command

- Show all images:
  `docker images`

- Processes, list of running containers:
  `docker ps`

- Stop a containers:
  `stop {image}:`
