mbentley/memcached
==================

docker image for memcached
Based off of stackbrew/debian:jessie

To pull this image:
`docker pull mbentley/memcached`

Example usage:
`docker run -itd -p 11211:11211 -p 11211:11211/udp mbentley/memcached`

By default, memcached starts with the following parameters: `-v -m 256 -p 11211 -c 1024`


You may override these by specifying them as the command, for example:

`docker run -itd -p 11211:11211 -p 11211:11211/udp mbentley/memcached -vv -m 512 -p 11211 -c 2048`
