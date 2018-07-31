# Angular Docker

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.1.1.

## How it works

Clone the repo
docker-compose up

### or (better)

Create an Angular Projekt
Copy the docker-compose.yml and the Dockerfile into the app folder
edit the two files for your project
and start with docker-compose up


## Further help

https://scotch.io/tutorials/create-a-mean-app-with-angular-2-and-docker-compose
https://mherman.org/blog/2018/02/26/dockerizing-an-angular-app/
https://angular.io/


## maybe important
Some information: if the docker container works fine but the startpage witth localhost:4200 does not work,
teke a look into the package.json. In this file under scripts, the start command needs the info the app is running on localhost.
edit the part of this file like this

```javascript
{
  "name": "my-app",
  "version": "0.0.0",
  "scripts": {
    "ng": "ng",
    "start": "ng serve --host 0.0.0.0",         #that is the important one

```