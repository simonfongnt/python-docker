# python-docker

## Build the image:
`sudo docker build --tag python-docker .`

## Tag image:
`sudo docker tag python-docker:latest python-docker:v1.0.0`

## Run image as a Container (mount ../core for python files updates):
`sudo docker run -t -d -v /volume1/project/python-docker/core:/app/core --name python-app python-docker`

## Reuse the Container:
`sudo docker restart python-app`
