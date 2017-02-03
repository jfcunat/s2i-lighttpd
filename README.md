# s2i-lighttpd

This is an [S2I](https://github.com/openshift/source-to-image) image use to build expose static web site with lighttpd


## Requirements

* [S2I](https://github.com/openshift/source-to-image)
* [Docker](https://www.docker.com/products/docker)


## To build the S2I image

	1. Clone this repository
	2. Execute ```docker build -t s2i-lighttpd .```

## To build an image with your application code

```s2i build git://<source code> s2i-lighttpd <application image>```

## To run your image with Docker

```docker run -it --rm <application image>```

The lighttpd server will listen on port 8080