# Docker

## Development
Building with a Dockerfile.env \
`docker build -f Dockerfile.env .`

Port forwarding \
`docker run -p <LocalMachine Port>:<Docker Port> <docker_image>`

For linking the local machine folders to the docker: \
`docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app 93369c946102`

Run tests on running container without docker-compose \
`docker exec -it 5f0bc19da4dc npm run test`
