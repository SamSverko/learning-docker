# create image with Alpine Linux OS
FROM alpine:3.7

# install node.js and npm
RUN apk add --update nodejs nodejs-npm

# make learning-docker-app folder directory
RUN mkdir /home/learning-docker-app

# copy local files to folder in Docker image
COPY . /home/learning-docker-app

# change working directory to folder with files
WORKDIR /home/learning-docker-app

# update npm modules
RUN npm i

# expose container to http traffic
EXPOSE 80
