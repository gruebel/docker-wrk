# wrk

[![Build Status](https://travis-ci.org/gruebel/docker-wrk.svg?branch=master)](https://travis-ci.org/gruebel/docker-wrk)
[![Docker Automated build](https://img.shields.io/docker/automated/gruebel/wrk.svg)](https://hub.docker.com/r/gruebel/wrk/builds/)

## Overview
A small image for HTTP benchmarking.
Based on the official Alpine image and build via multi-stage build. Additionally it is compressed with my upx container to make the image as small as possible **~5.5MB**
For more information on the great tool wrk check out their [GitHub project](https://github.com/wg/wrk)!

## Usage
### CMD
To start a simple benchmark test against a website run following command
```bash
$ docker run --rm gruebel/wrk:latest -t2 -c200 -d10s https://www.example.com
```
For further details on the parameters
```bash
$ docker run --rm gruebel/wrk:latest --help
```
