# docker-chrome

Runs Chrome in Docker and displays it to a remote X11 server

## Requirements

- Docker
- X11 Server - e.g. XQuartz for MacOSX

## Usage

```
git clone https://github.com/bbartolome/docker-chrome.git
cd docker-chrome
docker build -t bbartolome/docker-chrome .
docker run --privileged -it --rm -e DISPLAY=`hostname`:0 bbartolome/docker-chrome
```
