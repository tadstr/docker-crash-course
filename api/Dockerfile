# Initial Layer
# Pull image from DockerHub repo or our own computer
FROM node:17-alpine

RUN yarn global add nodemon

# Run every command below start in /app directory
WORKDIR /app

COPY package.json .

RUN yarn

# Copy from this current directory to /app because of WORKDIR
COPY . .

EXPOSE 4000

# Run at runtime when container begin to run
CMD ["yarn", "dev"] 