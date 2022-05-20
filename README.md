# docker cheet sheet

## build the node image

> docker build -t dhe/node16 .

> docker run -p 4200:8080 -v ${pwd}/usr/app -d dhe/node16


> docker run -p 49160:8080 -v ${pwd}/usr/app -d dhe/node16

## How to run a shell on a stopped container
### if you want to inspect your container , e.g. it did not start because "dir permission" failed in some instruction
### Start/run with a different entry point:
docker run -ti --entrypoint=sh user/test_image


## Rename docker image
[Rename docker image](Rename%20Docker%20Images%20Without%20Rebuilding)
