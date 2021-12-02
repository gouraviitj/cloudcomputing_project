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
 
## Detailed Process


1. We started out by installing VirtualBox application on our host machine in order to be able to run a virtual machine on VirtualBox.

2. After installing the VirtualBox we went ahead and downloaded the ubuntu 20.04 LTS iso image in order to run a linux-ubuntu based operating system on our virtual machine    	powered by VirtualBox.

3. We then completed setting up the VM by allocating the RAM size, hard disk space and other permission settings.

4. Finally, we then powered up the Virtual machine which was running using the path to the ubuntu based iso image.

5. After the Vm was up and running we then went ahead and installed Ububtu 20.04 LTS as the operating system for the virtual machine. It did include the steps like creating 	administrator accounts and selecting add ons that come with the OS.

6. The next step after the OS was installed in our Virtual machine’s operating system was to install all the required dependencies and libraries on the OS.

7. We went ahead at first and installed the pip packet manager using the command: - -	- 	sudo apt-get install python-pip3

8. After installing the pip packet manager we went ahead and installed docker using the following command: 
	-sudo apt install docker.io

9. Once we had docker in place, it was now time to connect our docker in the VM with the docker hub cloud account that we had on https://hub.docker.com

10. For this we used the command - docker login and entered our username and password

11. After logging into our docker hub account, it was now time to pull images from docker hub that catered to the TICK stack.

12. We used the following command to pull the respective four components of the TICK stack:
	-docker pull telegraf
	-docker pull kapacitor
	-docker pull influxdb
	-docker pull chronograf

13.After pulling the images from docker hub we checked the status of the images using the following command :
	-docker images

14.Once we confirmed that we had all the necessary images are in place, we then went ahead and started creating all the necessary containers that depict all the four 	    	different components of the TICK stack.

15. In order to run the container we used the following commands:
	-docker run telegraph
	-docker run kapacitor
	-docker run influxdb
	-docker run chronograf

16. After we entered and run the above command we were able to launch and run the docker container for all the different four components of the TICK stack.

17. Finally, then we went ahead and checked the status of the container using the following command:
	-docker container ls
	
18.	The process was viewed and tracked in the localhost url using chronograf.





