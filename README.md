# Udacity FSND Docker-based Vagrant replacement

## Use from Docker Hub
Change into the directory containing the code which you want to run in the context of the container, and enter:
```
docker run -it -v $PWD:/vagrant -p 5000:5000/tcp -p 8000:8000/tcp -p 8080:8080/tcp helmuthb/fullstack-nanodegree
```

You will be inside a Ubuntu 16.04-based container, as user `vagrant`. The user has sudo-rights (password is `vagrant` as well).

## Build the docker image
Execute this command to create the template:
```
docker build -t udacity .
```

## Run the docker image
Change into the folder which should be added to the vagrant file.
Execute the image interactively using:
```
docker run -v $PWD:/vagrant -p 5000:5000/tcp -p 8000:8000/tcp -p 8080:8080/tcp -it udacity
```
