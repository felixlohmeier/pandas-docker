# Docker container for Pandas

[pandas](http://pandas.pydata.org/) is an open source library providing data analysis tools for the Python programming language. This docker image contains pandas 0.20.3 and is build on top of the official python 3.6.3 slim image.

* [GitHub Repository with Dockerbuild files](https://github.com/felixlohmeier/pandas-docker)
* [Docker Hub with docker images](https://hub.docker.com/r/felixlohmeier/pandas/)

## fixed versions

* Python 3.6.3
* Pandas 0.20.3

## usage

### python console

> docker run -it --rm felixlohmeier/pandas

### run a script

> docker run --rm -v "$PWD":/data:z -w /data felixlohmeierpandas python my-script.py
