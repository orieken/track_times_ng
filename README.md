# track_times_ng
playing around with express and angular

## Build

## Deps

* Express
* Mocha
* Chai
* Bower
* Angular 
* Bootstrap


## docker 

* I uses this to build my [image](https://docs.docker.com/examples/nodejs_web_app/)
* docker run -p <port you map>:3000 -d orieken/node-track-times-ng
* curl -i $(boot2docker ip):<port you map>
* check ip with boot2docker ip

### code changes

right now I have to rebuild the container to add changes since the code gets copied to the container 
and im not sharing a folder

```
docker stop <conatiner hash>
docker build -t orieken/node-track-times-ng .
docker run -p <port you map>:3000 -d orieken/node-track-times-ng
```

### more reading

* [boot2docker exercise](https://docs.docker.com/installation/mac/)
* [nodejs app with docker](http://thenewstack.io/examples-of-building-a-node-js-app-with-docker/)
* [getting started with docker for nodejs dev](https://www.airpair.com/node.js/posts/getting-started-with-docker-for-the-nodejs-dev)
* [docker image cheatsheet](https://developer.basespace.illumina.com/docs/content/documentation/native-apps/manage-docker-image)
* [docker install and getting started](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-getting-started)
* [docker hot code deploys](http://blog.ionic.io/docker-hot-code-deploys/)


### for error
 
 ```
 Sending build context to Docker daemon 
 An error occurred trying to connect:
 ```
 
 try: [boot2docker](https://gist.github.com/garthk/d5a17007c277aa5c76de)
 
## To Dos

* docker/vagrant?
* codeship
* set up deployment 


### running
 
 ```
 boot2docker start
 ```
 
