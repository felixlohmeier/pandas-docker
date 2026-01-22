# Docker container for Pandas

[pandas](http://pandas.pydata.org/) is an open source library providing data analysis tools for the Python programming language. This docker image contains pandas and is build on top of the official python slim image.

* [GitHub Repository with Dockerbuild files](https://github.com/felixlohmeier/pandas-docker)
* [Docker Hub with docker images](https://hub.docker.com/r/felixlohmeier/pandas/)

## Available Tags

* 3.0.0: Pandas 3.0.0, Python 3.12.1
* 1.3.3: Pandas 1.3.3, Python 3.9.7
* 0.20.3: Pandas 0.20.3, Python 3.6.3

## Usage

### Python console

> docker run -it --rm felixlohmeier/pandas:1.3.3

### Run a script

> docker run --rm -v "$PWD":/data:z -w /data felixlohmeier/pandas:1.3.3 python my-script.py

## Development

```
cd 1.3.3
docker build -t felixlohmeier/pandas:1.3.3 .
docker login --username felixlohmeier --password X docker.io
docker push felixlohmeier/pandas:1.3.3
```

Manually update README in [Docker Hub Repo](https://hub.docker.com/repository/docker/felixlohmeier/pandas)
