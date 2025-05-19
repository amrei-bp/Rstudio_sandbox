# Rstudio_sandbox
This repository contains a gitpod environment to play with the docker image containing Rstudio and tidyverse.


[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/amrei-bp/Rstudio_sandbox)

This [Gitpod](https://www.gitpod.io/) environment (a docker container) comes installed with:
- Git
- Docker
- Pixi

To open the gitpod press the button above. If you are logged into Github it will open automatically. Otherwise log in. 

The environment in Gitpod contains a container image from [seqera containers](https://seqera.io/containers/). 

To list the images already in the container:
docker image ls

To start the container with interactive terminal: 
docker run --rm -it imageID bash

Take the imageID that is provided in the listed images. 

Now you can use R within the container. 

To exit the container:
exit
