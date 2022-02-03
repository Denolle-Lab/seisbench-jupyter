# docker-template
This repository builds a [JupyterHub](https://jupyter.org/hub) environment with Repo2Docker [GitHub Actions CI](https://github.com/jupyterhub/repo2docker-action)

[![Action Status](https://github.com/Denolle-Lab/seisbench-jupyter/workflows/CI/badge.svg)](https://github.com/Denolle-Lab/seisbench-jupyter/actions)
[![Docker Pulls](https://img.shields.io/docker/pulls/uwessds/seisbench)](https://hub.docker.com/r/uwessds/seisbench/tags)
[![BinderHub](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Denolle-Lab/seisbench-jupyter/HEAD?urlpath=lab)


### Pull your image to run a local JupyterLab session

You can run JupyterLab with this conda environment on any machine with [Docker Installed](https://docs.docker.com/get-docker/)

*set the $HOMEDIR environment variable to mount a local directory for JupyterLab to access*

```bash
git clone https://github.com/Denolle-Lab/seisbench-jupyter
cd seisbench-jupyter
export HOMEDIR=/tmp/data
docker compose up
# NOTE: ctrl-c will 'stop' the container, to fully shut down:
docker compose down
```

### Pull image from respository

* From [DockerHub](https://hub.docker.com/r/uwessds/seisbench/tags): `docker pull uwessds/seisbench:latest`
