## Setup

### Prerequisites
There are no specific skills needed for this tutorial beyond a basic comfort with the command line and using a text editor. Prior experience in developing web applications will be helpful but is not required. As you proceed further along the tutorial, we'll make use of [Play With Docker](https://labs.play-with-docker.com/).

Login to Play With Docker website requires a [Docker Hub](https://hub.docker.com/) account. Please make sure you get registered on [Docker Hub](https://hub.docker.com/) to proceed further.

### Setting up your computer
Getting all the tooling setup on your computer can be a daunting task, but getting Docker up and running on your favorite OS has become very easy.

The *getting started* guide on Docker has detailed instructions for setting up Docker on [Mac](https://docs.docker.com/docker-for-mac/), [Linux](https://docs.docker.com/engine/installation/linux/) and [Windows](https://docs.docker.com/docker-for-windows/).

*If you're using Docker for Windows* make sure you have [shared your drive](https://docs.docker.com/docker-for-windows/#shared-drives).

*Important note* If you're using an older version of Windows or MacOS you may need to use [Docker Machine](https://docs.docker.com/machine/overview/) instead.

*All commands work in either bash or Powershell on Windows*

### Check your environment

*When you are successfully logged into PWD website you get an active session for 4hrs. Make sure you don't close this browser window for the period you finish this lab session.*


```
$ docker run hello-world
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
03f4658f8b78: Pull complete
a3ed95caeb02: Pull complete
Digest: sha256:8be990ef2aeb16dbcb9271ddfe2610fa6658d13f6dfb8bc72074cc1ca36966a7
Status: Downloaded newer image for hello-world:latest

Hello from Docker.
This message shows that your installation appears to be working correctly.
...
```

![Hello world explainer](images/ops-basics-hello-world.svg)
If you are familiar with VMs, you may be thinking this is pretty much just like running a virtual machine, except with a central repository of VM images. And in this simple example, that is basically true. But as you go through these exercises you will start to see important ways that Docker and containers differ from VMs. For now, the simple explanation is this:
* The VM is a *hardware* abstraction: it takes physical CPUs and RAM from a host, and divides and shares it across several smaller virtual machines. There is an OS and application running inside the VM, but the virtualization software usually has no real knowledge of that.
* A container is an *application* abstraction: the focus is really on the OS and the application, and not so much the hardware abstraction.
Many customers actually use both VMs and containers today in their environments and, in fact, may run containers inside of VMs. 

## Next Steps
For the next step in the tutorial, head over to [1.0 Running your first container](alpine.md)
