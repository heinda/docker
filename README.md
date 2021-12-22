# docker cheet sheet

## build the node image

> docker build -t dhe/node16 .

> docker run -p 4200:8080 -v ${pwd}/usr/app -d dhe/node16


> docker run -p 49160:8080 -v ${pwd}/usr/app -d dhe/node16