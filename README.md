[![Docker pulls](https://img.shields.io/docker/pulls/dlanguage/gdc.svg)](https://hub.docker.com/r/dlanguage/gdc/)
[![Docker Build](https://img.shields.io/docker/automated/dlanguage/gdc.svg)](https://hub.docker.com/r/dlanguage/gdc/)

# docker-gdc

Docker Image for GDC

## Usage

Place a `test.d` in your current directory.
Then execute
```
docker run --rm -ti \
  -e USER -e HOME -e LOCAL_USER_ID=`id -u $USER` -e LOCAL_GROUP_ID=`id -g $USER`
  -w $(pwd) \
  -v /home/$USER:/home/$USER \
  dlanguage/gdc gdc test.d
```
