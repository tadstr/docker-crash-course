# Initial Layer
# Pull image from DockerHub repo or our own computer
FROM node:17-alpine

# Run every command below start in /app directory
WORKDIR /app

# Copy from this current directory to /app because of WORKDIR
COPY . .

RUN yarn

EXPOSE 4000

# Run at runtime when container begin to run
CMD ["node", "app.js"]

## CREATE THE IMAGE
# docker build -t my-express-app .

## RUN THE IMAGE (crate new container)
# docker run --name express-cli -p 4000:4000 -d my-express-app
# -p: publish to localhost port
# -d: detach

## START THE CONTAINER (existed)
# docker start express-cli (names)

## CLI
# docker images: show all images
# docker ps: processes, list of running containers
# stop {image}: stop a container