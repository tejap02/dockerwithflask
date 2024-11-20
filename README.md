# Docker Implementation of Python Flask Based Application



ssh-keygen -t rsa -b 4096 -C "info@nubeera.com" -f /root/.ssh/lk

mv lk.pub lock.pub
mv lk key

cat /root/.ssh/lock.pub

Add Key to [github.com](https://github.com/settings/keys)

eval $(ssh-agent -s)

ssh-add /root/.ssh/key

cd ~/~

git clone git@github.com:NubeEra-MCO/PythonFlaskDocker.git

cd PythonFlaskDocker

## Build Docker Custom Image
docker build -t custom-img-pyapp .

## Verify Docker Image
docker image ls

## Run Custom Image into Container
docker run --rm -p 8000:8000 custom-img-pyapp:v2


# V2
##########################################
$ git pull

$ docker rmi custom-img-pyapp:v2 --force

$ docker build -t custom-img-pyapp:v2 .

$ docker image ls



