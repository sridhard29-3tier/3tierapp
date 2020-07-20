# Sample 3tier app
This repo contains code for a Node.js multi-tier application.

The application overview is as follows

```
web <=> api <=> db
```

The folders `web` and `api` respectively describe how to install and run each app.

## Bringing up the development environment
The development environment for this application can be brought up with docker compose. In order run this environment it's necessary to checkout [web app] into the parent directory of this repo.
```
$ pwd
/home/ubuntu/projects/3tierapp
$ tree -L 1
.
├── 3tierapp-app
└── 3tierapp-web

2 directories, 0 files
```
Changes can be made to either the web or api tier of this application by editing either the web repo or this one. When ready to run this application locally
do the following in the root of this repo:
```
docker-compose build
docker-compose up
```


## Infrastructure and CI/CD pipeline 
For more information on building the infrastructure and CI/CD pipeline view the [Infrastructure installation](INSTALL.md)

