# Cloud Computing Project 
# Q.no 1 - TICK Stack

This document serves as a readme guide to the cloud computing end term project  question Number 1.

## Authors:

- Roll Number - MT19AIE212
- Name - Anindya Kumar Parida

- Roll Number - MT19AIE237
- Name - Gourav Sanghai

  
## Host Configuration:

 - Host operating system used - Mac OS/ Linux
 - Hypervisor used - [Virtualbox](https://www.virtualbox.org/)
 - VM operating system - Ububtu 20.04 LTS
 - WSL2
 

## Brief Process:
1. Download the image file from docker hub


## Process | Step 1 

- First of all we start out by creating our own base os image and do not make any use of base os images that are available on Docker Hub. We create our own base os image of the ubuntu 20.04 os from scratch.
- Inorder to create our own base os image, we first download the ubuntu-base-20.04-base-amd.tar.gz OS file from this [link.](ubuntu-base-20.04.1-base-amd64.tar.gz)
- After we download the ubuntu-base-20.04-base-amd.tar.gz file from the above link, we now go ahead create our own base os image using the downloaded file.
- Please note to keep the downloaded file and "Dockerfile" at the same file path. I have not uploaded the large file here on github. 
- we will also make a folder named "apache2docker" and keep all our files here. We also move the downloaded file to this folder.
- Inorder to create our own base os image we will create a file with the name "Dockerfile" and write the following code in mac terminal

## Installation | Step -1 | Create base image from scratch

Making a folder to manage files properly

```bash
  mkdir apache2docker
  cd apache2docker
```

Create a file named "Dockerfile"
```bash
sudo nano Dockerfile
```

Write the following code in Dockerfile to create a base os image and save the file
- Ensure that "ubuntu-base-20.04.1-base-amd64.tar.gz" and "Dockerfile" are on the same file path
```bash
FROM scratch
LABEL org.label-schema.schema-version="1.0" \
	org.label-schema.name="Ubuntu Base Image" \
	maintainer="gouravsanghai" \
	org.label-schema.vcs-description="ubuntu Base Image-minimal"\
	org.label.schema.docker.cmd="docker run -it ubuntu sh" \
	org.label-schema.vendor="ubuntu" \
	org.label-schema.license="GPLv2" \
	org.label-schema.build-date="20190801"
ADD ubuntu-base-20.04.1-base-amd64.tar.gz /
CMD ["/bin/bash"]

```
