# Udacity FSND Docker-based Vagrant replacement

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
