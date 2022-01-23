# HelloWorld (Docker)

## 0. Table of Contents
- [HelloWorld (Docker)](#helloworld-docker)
  - [0. Table of Contents](#0-table-of-contents)
  - [1. How to Setup in a Mac M1 laptop?](#1-how-to-setup-in-a-mac-m1-laptop)
  - [2. References](#2-references)

## 1. How to Setup in a Mac M1 laptop?

1. Install **Docker Desktop** via **Homebrew**.
   - **Command**: `brew install --cask docker`
   - **Homebrew Link**: https://formulae.brew.sh/cask/docker#default

2. Open **Docker Desktop** & Ensure it is running.

3. Start a new container called `helloworld` to run an image called `dockerinaction/hello_world`.
   - **Command**: 
        ```
        docker run \
            --platform linux/amd64 \
            --name helloworld \
            dockerinaction/hello_world
        ```

4. Delete the container named `helloworld`.
   - **Command**: `docker rm helloworld`

## 2. References

- [Homebrew - docker](https://formulae.brew.sh/cask/docker#default)