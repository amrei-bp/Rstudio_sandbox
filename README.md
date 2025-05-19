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

## Rstudio in browser

To run the rstudio graphical user interface you can make use of [The Rocker Project](https://rocker-project.org/), where they have built a variety of Docker containers for R. 

You can start the rstudio instance with 

```{.bash}
docker run --rm -ti -e PASSWORD=yourpassword -p 8787:8787 rocker/rstudio
```

When running from within the gitpod you will get a little pop-up asking you to open `port 8787`, say yes. 

Then there will be another pop-up (kill process with ctrl + c and start with the docker run command again if it doesn't pop up) where you need to say you want to run in the browser. 

In the browser window that opens up the user name will be `root`, the password `yourpassword`. Once you are logged in you can use Rstudio in your browser. 

To start a Rstudio session outside of Gitpod you need to have docker installed. 
