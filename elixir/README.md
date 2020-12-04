<!--

********************************************************************************

WARNING:

    DO NOT EDIT "elixir/README.md"

    IT IS AUTO-GENERATED

    (from the other files in "elixir/" combined with a set of templates)

********************************************************************************

-->

**Note:** this is the "per-architecture" repository for the `ppc64le` builds of [the `elixir` official image](https://hub.docker.com/_/elixir) -- for more information, see ["Architectures other than amd64?" in the official images documentation](https://github.com/docker-library/official-images#architectures-other-than-amd64) and ["An image's source changed in Git, now what?" in the official images FAQ](https://github.com/docker-library/faq#an-images-source-changed-in-git-now-what).

# Quick reference

-	**Maintained by**:  
	[the Docker Community](https://github.com/c0b/docker-elixir), [with Elixir's support](https://github.com/docker-library/official-images/pull/1398#issuecomment-180484549)

-	**Where to get help**:  
	[the Docker Community Forums](https://forums.docker.com/), [the Docker Community Slack](https://dockr.ly/slack), or [Stack Overflow](https://stackoverflow.com/search?tab=newest&q=docker)

# Supported tags and respective `Dockerfile` links

-	[`1.11.2`, `1.11`, `latest`](https://github.com/erlef/docker-elixir/blob/f226e68615d6955ee311b8d613c3c8ca843e9f51/1.11/Dockerfile)
-	[`1.11.2-slim`, `1.11-slim`, `slim`](https://github.com/erlef/docker-elixir/blob/f226e68615d6955ee311b8d613c3c8ca843e9f51/1.11/slim/Dockerfile)
-	[`1.11.2-alpine`, `1.11-alpine`, `alpine`](https://github.com/erlef/docker-elixir/blob/f226e68615d6955ee311b8d613c3c8ca843e9f51/1.11/alpine/Dockerfile)
-	[`1.10.4`, `1.10`](https://github.com/erlef/docker-elixir/blob/a8d582c328db5864a4e8e5f869900e3a52265f38/1.10/Dockerfile)
-	[`1.10.4-slim`, `1.10-slim`](https://github.com/erlef/docker-elixir/blob/a8d582c328db5864a4e8e5f869900e3a52265f38/1.10/slim/Dockerfile)
-	[`1.10.4-alpine`, `1.10-alpine`](https://github.com/erlef/docker-elixir/blob/a8d582c328db5864a4e8e5f869900e3a52265f38/1.10/alpine/Dockerfile)
-	[`1.9.4`, `1.9`](https://github.com/erlef/docker-elixir/blob/0d9f47458468a8bf1407374731cbec077ab6f895/1.9/Dockerfile)
-	[`1.9.4-slim`, `1.9-slim`](https://github.com/erlef/docker-elixir/blob/0d9f47458468a8bf1407374731cbec077ab6f895/1.9/slim/Dockerfile)
-	[`1.9.4-alpine`, `1.9-alpine`](https://github.com/erlef/docker-elixir/blob/0d9f47458468a8bf1407374731cbec077ab6f895/1.9/alpine/Dockerfile)

[![ppc64le/elixir build status badge](https://img.shields.io/jenkins/s/https/doi-janky.infosiftr.net/job/multiarch/job/ppc64le/job/elixir.svg?label=ppc64le/elixir%20%20build%20job)](https://doi-janky.infosiftr.net/job/multiarch/job/ppc64le/job/elixir/)

# Quick reference (cont.)

-	**Where to file issues**:  
	[https://github.com/c0b/docker-elixir/issues](https://github.com/c0b/docker-elixir/issues)

-	**Supported architectures**: ([more info](https://github.com/docker-library/official-images#architectures-other-than-amd64))  
	[`amd64`](https://hub.docker.com/r/amd64/elixir/), [`arm32v7`](https://hub.docker.com/r/arm32v7/elixir/), [`arm64v8`](https://hub.docker.com/r/arm64v8/elixir/), [`i386`](https://hub.docker.com/r/i386/elixir/), [`ppc64le`](https://hub.docker.com/r/ppc64le/elixir/), [`s390x`](https://hub.docker.com/r/s390x/elixir/)

-	**Published image artifact details**:  
	[repo-info repo's `repos/elixir/` directory](https://github.com/docker-library/repo-info/blob/master/repos/elixir) ([history](https://github.com/docker-library/repo-info/commits/master/repos/elixir))  
	(image metadata, transfer size, etc)

-	**Image updates**:  
	[official-images PRs with label `library/elixir`](https://github.com/docker-library/official-images/pulls?q=label%3Alibrary%2Felixir)  
	[official-images repo's `library/elixir` file](https://github.com/docker-library/official-images/blob/master/library/elixir) ([history](https://github.com/docker-library/official-images/commits/master/library/elixir))

-	**Source of this description**:  
	[docs repo's `elixir/` directory](https://github.com/docker-library/docs/tree/master/elixir) ([history](https://github.com/docker-library/docs/commits/master/elixir))

# What is Elixir?

Elixir is a dynamic, functional language designed for building scalable and maintainable applications.

Elixir leverages the Erlang VM, known for running low-latency, distributed and fault-tolerant systems, while also being successfully used in web development and the embedded software domain.

> [en.wikipedia.org/wiki/Elixir_(programming_language)](https://en.wikipedia.org/wiki/Elixir_%28programming_language%29)

![logo](https://raw.githubusercontent.com/docker-library/docs/f3ee5318992592f987a289cd72d63ac1807f569d/elixir/logo.png)

# How to use this image

## Run it as the REPL

```console
➸ docker run -it --rm ppc64le/elixir
Erlang/OTP 18 [erts-7.2.1] [source] [64-bit] [smp:8:8] [async-threads:10] [hipe] [kernel-poll:false]

Interactive Elixir (1.2.1) - press Ctrl+C to exit (type h() ENTER for help)
iex(1)> System.version
"1.2.1"
iex(2)>
➸ docker run -it --rm -h elixir.local ppc64le/elixir iex --sname snode
Erlang/OTP 18 [erts-7.2.1] [source] [64-bit] [smp:8:8] [async-threads:10] [hipe] [kernel-poll:false]

Interactive Elixir (1.2.1) - press Ctrl+C to exit (type h() ENTER for help)
iex(snode@elixir)1> System.version
"1.2.1"
iex(snode@elixir)2> :c.uptime
14 seconds
:ok
```

## Run a single Elixir exs script

```console
$ docker run -it --rm --name elixir-inst1 -v "$PWD":/usr/src/myapp -w /usr/src/myapp ppc64le/elixir elixir your-escript.exs
```

# Image Variants

The `ppc64le/elixir` images come in many flavors, each designed for a specific use case.

## `ppc64le/elixir:<version>`

This is the defacto image. If you are unsure about what your needs are, you probably want to use this one. It is designed to be used both as a throw away container (mount your source code and start the container to start your app), as well as the base to build other images off of.

## `ppc64le/elixir:<version>-slim`

This image does not contain the common packages contained in the default tag and only contains the minimal packages needed to run `ppc64le/elixir`. Unless you are working in an environment where *only* the `ppc64le/elixir` image will be deployed and you have space constraints, we highly recommend using the default image of this repository.

## `ppc64le/elixir:<version>-alpine`

This image is based on the popular [Alpine Linux project](https://alpinelinux.org), available in [the `alpine` official image](https://hub.docker.com/_/alpine). Alpine Linux is much smaller than most distribution base images (~5MB), and thus leads to much slimmer images in general.

This variant is highly recommended when final image size being as small as possible is desired. The main caveat to note is that it does use [musl libc](https://musl.libc.org) instead of [glibc and friends](https://www.etalabs.net/compare_libcs.html), so certain software might run into issues depending on the depth of their libc requirements. However, most software doesn't have an issue with this, so this variant is usually a very safe choice. See [this Hacker News comment thread](https://news.ycombinator.com/item?id=10782897) for more discussion of the issues that might arise and some pro/con comparisons of using Alpine-based images.

To minimize image size, it's uncommon for additional related tools (such as `git` or `bash`) to be included in Alpine-based images. Using this image as a base, add the things you need in your own Dockerfile (see the [`alpine` image description](https://hub.docker.com/_/alpine/) for examples of how to install packages if you are unfamiliar).

# License

Copyright 2012 Plataformatec

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

View [license information](http://www.apache.org/licenses/LICENSE-2.0) for the software contained in this image.

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

As with all Docker images, these likely also contain other software which may be under other licenses (such as Bash, etc from the base distribution, along with any direct or indirect dependencies of the primary software being contained).

Some additional license information which was able to be auto-detected might be found in [the `repo-info` repository's `elixir/` directory](https://github.com/docker-library/repo-info/tree/master/repos/elixir).

As for any pre-built image usage, it is the image user's responsibility to ensure that any use of this image complies with any relevant licenses for all software contained within.
