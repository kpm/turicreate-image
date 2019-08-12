# Turi Create Image
![Docker Pulls](https://img.shields.io/docker/pulls/kristianp/turicreate?style=for-the-badge)
[![](https://images.microbadger.com/badges/image/kristianp/turicreate.svg)](https://microbadger.com/images/kristianp/turicreate "Get your own image badge on microbadger.com")

This is a fork of https://github.com/houtzager/turicreate-image .  This fork is based on Ubuntu 18.04, and runs on python3, without any virtualenv, so remember to use python3 and pip3 in commands.


This repository contains a Docker image for running Turi Create scripts.  This fork also contains jupyterlab notebook, so turicreate can be used in a jupyter notebook.

# Usage
```bash
docker run --rm -v /my/volume/directory/:/workdir/ kristianp/turicreate -p 8888:8888 jupyter notebook --ip=0.0.0.0 --allow-root
```

The run configuration example described above could be used for running a Turi Create script located in your workdir. The container will remove itself as soon as it's finished.

# References
Docker Hub: https://hub.docker.com/r/kristianp/turicreate

Turi Create Repo: https://github.com/apple/turicreate
