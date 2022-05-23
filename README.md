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

## How to save and load an image

Save the Docker image as a tar file:
```
> docker save -o <path for generated tar file> <image name>

´´´
  Then copy your image to a new system with regular file transfer tools such as cp, scp or rsync(preferred for big files). After that you will have to load the image into Docker:
  
```
> docker load -i <path to image tar file>
  
´´´
  # docker commit a running container 
  
  sudo docker commit -p deddd39fa163 new:version
