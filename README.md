# Udagram Image Filtering Microservice

Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.



### Installing project dependencies

This project uses NPM to manage software dependencies. NPM Relies on the package.json file located in the root of this repository. After cloning, open your terminal and run:
```bash
npm install
```


### Setup Backend Node Environment
1. Initialize a new project: `npm init`
2. Install express: `npm i express --save`
3. Install typescript dependencies: `npm i ts-node-dev tslint typescript  @types/bluebird @types/express @types/node --save-dev`



### Docker Configuration
docker-compose -f docker-compose-build.yaml build --parallel

docker-compose up

***
### Kuberentes configuration
kubectl apply -f backend-feed-deployment.yaml 

kubectl apply -f backend-user-deployment.yaml 

kubectl apply -f frontend-deployment.yaml 

kubectl apply -f reverseproxy-deployment.yaml

kubectl apply -f pod-example/pod.yaml
