<!--

********************************************************************************

WARNING:

    DO NOT EDIT "python/README.md"

    IT IS AUTO-GENERATED

    (from the other files in "python/" combined with a set of templates)

********************************************************************************

-->

**Note:** this is the "per-architecture" repository for the `arm32v5` builds of [the `python` official image](https://hub.docker.com/_/python) -- for more information, see ["Architectures other than amd64?" in the official images documentation](https://github.com/docker-library/official-images#architectures-other-than-amd64) and ["An image's source changed in Git, now what?" in the official images FAQ](https://github.com/docker-library/faq#an-images-source-changed-in-git-now-what).

# Quick reference

-	**Maintained by**:  
	[the Docker Community](https://github.com/docker-library/python)

-	**Where to get help**:  
	[the Docker Community Forums](https://forums.docker.com/), [the Docker Community Slack](https://dockr.ly/slack), or [Stack Overflow](https://stackoverflow.com/search?tab=newest&q=docker)

# Supported tags and respective `Dockerfile` links

(See ["What's the difference between 'Shared' and 'Simple' tags?" in the FAQ](https://github.com/docker-library/faq#whats-the-difference-between-shared-and-simple-tags).)

## Simple Tags

-	[`3.10.0a2-buster`, `3.10-rc-buster`, `rc-buster`](https://github.com/docker-library/python/blob/dc9b64baf4c01bad4ddca590418dcfdb46a13ac2/3.10-rc/buster/Dockerfile)
-	[`3.10.0a2-slim-buster`, `3.10-rc-slim-buster`, `rc-slim-buster`, `3.10.0a2-slim`, `3.10-rc-slim`, `rc-slim`](https://github.com/docker-library/python/blob/dc9b64baf4c01bad4ddca590418dcfdb46a13ac2/3.10-rc/buster/slim/Dockerfile)
-	[`3.9.0-buster`, `3.9-buster`, `3-buster`, `buster`](https://github.com/docker-library/python/blob/ed08d468b219d19de869ba669bc4e91e2dc00cb3/3.9/buster/Dockerfile)
-	[`3.9.0-slim-buster`, `3.9-slim-buster`, `3-slim-buster`, `slim-buster`, `3.9.0-slim`, `3.9-slim`, `3-slim`, `slim`](https://github.com/docker-library/python/blob/ed08d468b219d19de869ba669bc4e91e2dc00cb3/3.9/buster/slim/Dockerfile)
-	[`3.8.6-buster`, `3.8-buster`](https://github.com/docker-library/python/blob/f50263f4338cc41882aa0675e3ce257c7314d425/3.8/buster/Dockerfile)
-	[`3.8.6-slim-buster`, `3.8-slim-buster`, `3.8.6-slim`, `3.8-slim`](https://github.com/docker-library/python/blob/f50263f4338cc41882aa0675e3ce257c7314d425/3.8/buster/slim/Dockerfile)
-	[`3.7.9-buster`, `3.7-buster`](https://github.com/docker-library/python/blob/bc9f6c85c155a7aeb6a308c3399c9134223f0370/3.7/buster/Dockerfile)
-	[`3.7.9-slim-buster`, `3.7-slim-buster`, `3.7.9-slim`, `3.7-slim`](https://github.com/docker-library/python/blob/bc9f6c85c155a7aeb6a308c3399c9134223f0370/3.7/buster/slim/Dockerfile)
-	[`3.7.9-stretch`, `3.7-stretch`](https://github.com/docker-library/python/blob/bc9f6c85c155a7aeb6a308c3399c9134223f0370/3.7/stretch/Dockerfile)
-	[`3.7.9-slim-stretch`, `3.7-slim-stretch`](https://github.com/docker-library/python/blob/bc9f6c85c155a7aeb6a308c3399c9134223f0370/3.7/stretch/slim/Dockerfile)
-	[`3.6.12-buster`, `3.6-buster`](https://github.com/docker-library/python/blob/c15acf875a4d4ae760bcd793742906873fd9e57b/3.6/buster/Dockerfile)
-	[`3.6.12-slim-buster`, `3.6-slim-buster`, `3.6.12-slim`, `3.6-slim`](https://github.com/docker-library/python/blob/c15acf875a4d4ae760bcd793742906873fd9e57b/3.6/buster/slim/Dockerfile)
-	[`3.6.12-stretch`, `3.6-stretch`](https://github.com/docker-library/python/blob/c15acf875a4d4ae760bcd793742906873fd9e57b/3.6/stretch/Dockerfile)
-	[`3.6.12-slim-stretch`, `3.6-slim-stretch`](https://github.com/docker-library/python/blob/c15acf875a4d4ae760bcd793742906873fd9e57b/3.6/stretch/slim/Dockerfile)

## Shared Tags

-	`3.10.0a2`, `3.10-rc`, `rc`:
	-	[`3.10.0a2-buster`](https://github.com/docker-library/python/blob/dc9b64baf4c01bad4ddca590418dcfdb46a13ac2/3.10-rc/buster/Dockerfile)
-	`3.9.0`, `3.9`, `3`, `latest`:
	-	[`3.9.0-buster`](https://github.com/docker-library/python/blob/ed08d468b219d19de869ba669bc4e91e2dc00cb3/3.9/buster/Dockerfile)
-	`3.8.6`, `3.8`:
	-	[`3.8.6-buster`](https://github.com/docker-library/python/blob/f50263f4338cc41882aa0675e3ce257c7314d425/3.8/buster/Dockerfile)
-	`3.7.9`, `3.7`:
	-	[`3.7.9-buster`](https://github.com/docker-library/python/blob/bc9f6c85c155a7aeb6a308c3399c9134223f0370/3.7/buster/Dockerfile)
-	`3.6.12`, `3.6`:
	-	[`3.6.12-buster`](https://github.com/docker-library/python/blob/c15acf875a4d4ae760bcd793742906873fd9e57b/3.6/buster/Dockerfile)

[![arm32v5/python build status badge](https://img.shields.io/jenkins/s/https/doi-janky.infosiftr.net/job/multiarch/job/arm32v5/job/python.svg?label=arm32v5/python%20%20build%20job)](https://doi-janky.infosiftr.net/job/multiarch/job/arm32v5/job/python/)

# Quick reference (cont.)

-	**Where to file issues**:  
	[https://github.com/docker-library/python/issues](https://github.com/docker-library/python/issues)

-	**Supported architectures**: ([more info](https://github.com/docker-library/official-images#architectures-other-than-amd64))  
	[`amd64`](https://hub.docker.com/r/amd64/python/), [`arm32v5`](https://hub.docker.com/r/arm32v5/python/), [`arm32v6`](https://hub.docker.com/r/arm32v6/python/), [`arm32v7`](https://hub.docker.com/r/arm32v7/python/), [`arm64v8`](https://hub.docker.com/r/arm64v8/python/), [`i386`](https://hub.docker.com/r/i386/python/), [`mips64le`](https://hub.docker.com/r/mips64le/python/), [`ppc64le`](https://hub.docker.com/r/ppc64le/python/), [`s390x`](https://hub.docker.com/r/s390x/python/), [`windows-amd64`](https://hub.docker.com/r/winamd64/python/)

-	**Published image artifact details**:  
	[repo-info repo's `repos/python/` directory](https://github.com/docker-library/repo-info/blob/master/repos/python) ([history](https://github.com/docker-library/repo-info/commits/master/repos/python))  
	(image metadata, transfer size, etc)

-	**Image updates**:  
	[official-images PRs with label `library/python`](https://github.com/docker-library/official-images/pulls?q=label%3Alibrary%2Fpython)  
	[official-images repo's `library/python` file](https://github.com/docker-library/official-images/blob/master/library/python) ([history](https://github.com/docker-library/official-images/commits/master/library/python))

-	**Source of this description**:  
	[docs repo's `python/` directory](https://github.com/docker-library/docs/tree/master/python) ([history](https://github.com/docker-library/docs/commits/master/python))

# What is Python?

Python is an interpreted, interactive, object-oriented, open-source programming language. It incorporates modules, exceptions, dynamic typing, very high level dynamic data types, and classes. Python combines remarkable power with very clear syntax. It has interfaces to many system calls and libraries, as well as to various window systems, and is extensible in C or C++. It is also usable as an extension language for applications that need a programmable interface. Finally, Python is portable: it runs on many Unix variants, on the Mac, and on Windows 2000 and later.

> [wikipedia.org/wiki/Python_(programming_language)](https://en.wikipedia.org/wiki/Python_%28programming_language%29)

![logo](https://raw.githubusercontent.com/docker-library/docs/01c12653951b2fe592c1f93a13b4e289ada0e3a1/python/logo.png)

# How to use this image

## Create a `Dockerfile` in your Python app project

```dockerfile
FROM arm32v5/python:3

WORKDIR /usr/src/app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD [ "python", "./your-daemon-or-script.py" ]
```

or (if you need to use Python 2):

```dockerfile
FROM arm32v5/python:2

WORKDIR /usr/src/app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD [ "python", "./your-daemon-or-script.py" ]
```

You can then build and run the Docker image:

```console
$ docker build -t my-python-app .
$ docker run -it --rm --name my-running-app my-python-app
```

## Run a single Python script

For many simple, single file projects, you may find it inconvenient to write a complete `Dockerfile`. In such cases, you can run a Python script by using the Python Docker image directly:

```console
$ docker run -it --rm --name my-running-script -v "$PWD":/usr/src/myapp -w /usr/src/myapp arm32v5/python:3 python your-daemon-or-script.py
```

or (again, if you need to use Python 2):

```console
$ docker run -it --rm --name my-running-script -v "$PWD":/usr/src/myapp -w /usr/src/myapp arm32v5/python:2 python your-daemon-or-script.py
```

## Multiple Python versions in the image

In the non `python:slim` variants there will be an additional older `python` executable at `/usr/bin/python` while the desired newer `/usr/local/bin/python` is the default choice in the `$PATH`. This is an unfortunate side-effect of using the `buildpack-deps` image in the non-slim variants

# Image Variants

The `arm32v5/python` images come in many flavors, each designed for a specific use case.

## `arm32v5/python:<version>`

This is the defacto image. If you are unsure about what your needs are, you probably want to use this one. It is designed to be used both as a throw away container (mount your source code and start the container to start your app), as well as the base to build other images off of.

Some of these tags may have names like buster or stretch in them. These are the suite code names for releases of [Debian](https://wiki.debian.org/DebianReleases) and indicate which release the image is based on. If your image needs to install any additional packages beyond what comes with the image, you'll likely want to specify one of these explicitly to minimize breakage when there are new releases of Debian.

This tag is based off of [`buildpack-deps`](https://hub.docker.com/_/buildpack-deps/). `buildpack-deps` is designed for the average user of Docker who has many images on their system. It, by design, has a large number of extremely common Debian packages. This reduces the number of packages that images that derive from it need to install, thus reducing the overall size of all images on your system.

## `arm32v5/python:<version>-slim`

This image does not contain the common packages contained in the default tag and only contains the minimal packages needed to run `arm32v5/python`. Unless you are working in an environment where *only* the `arm32v5/python` image will be deployed and you have space constraints, we highly recommend using the default image of this repository.

# License

View license information for [Python 2](https://docs.python.org/2/license.html) and [Python 3](https://docs.python.org/3/license.html).

As with all Docker images, these likely also contain other software which may be under other licenses (such as Bash, etc from the base distribution, along with any direct or indirect dependencies of the primary software being contained).

Some additional license information which was able to be auto-detected might be found in [the `repo-info` repository's `python/` directory](https://github.com/docker-library/repo-info/tree/master/repos/python).

As for any pre-built image usage, it is the image user's responsibility to ensure that any use of this image complies with any relevant licenses for all software contained within.
