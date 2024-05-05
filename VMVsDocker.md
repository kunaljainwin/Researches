# Overview and Context for this POC
In software development we need Environments/Setups throughout Software Development Lifecycle.
To create and manage these ENV on a any Physical machine, There are two ways :
1. Virtualization
2. Containerization

## Why ?
We need to compare them so that one can easily choose as per his/her requirements.

## Comparison 
### Basis of Implementation
<p>
Firstly for spinning a VM we need to run a software called Hypervisor on our Physical machine. Hypervisors offer full hardware virtualization, creating virtual machines (VMs) that run multiple operating systems on a single physical system. This approach allows for the simultaneous use of different operating systems and enables the management of multiple VMs from one system. However, this full virtualization comes at the cost of heavier resource consumption, as each VM requires its own set of resources.
</p>
<p>
Docker utilizes containerization to virtualize the operating system, rather than the hardware. Containers share the host system's kernel and other resources, making them more lightweight and efficient compared to VMs. Users can package applications and their dependencies into containers using Docker, allowing them to run on any Docker-enabled system. This approach is particularly well-suited for microservices architectures and cloud-native applications, where scalability and resource efficiency are crucial.
</p>

![image](https://github.com/kunaljainwin/my-notes/assets/72144717/427d2409-be58-4ac7-980c-e5e7714896ac)

:: Credits : Simplilearn
<p>
  While hypervisors enable the use of multiple operating systems on a single system and allow for different users to access the same resources in various ways, Docker containers are limited to running on a single operating system. However, containers offer fast boot times since they all run on the same host system and can share resources efficiently. Additionally, Docker containers do not have their own operating system; instead, they rely on the host operating system to create instances and provide parameters, allowing for flexibility and customization.
</p>

### Basis of Resource Utilization

#### Basic Setup: VM using Oracle Virtual Box and Vagrant and Docker using Docker desktop
- Orace VM: Ubuntu 20.04
![image](https://github.com/kunaljainwin/my-notes/assets/72144717/c77ae470-b162-4c45-9878-6ea6a5f277f8)
![image](https://github.com/kunaljainwin/my-notes/assets/72144717/5da2184d-4c97-4a9a-a3c1-52ce048ada24)
- Steps
  1. Install VM Virtual Box
  2. Install Vagrant (A VM management CLI tool) and Create a Vagrantfile
- output
![image](https://github.com/kunaljainwin/my-notes/assets/72144717/ab024fef-6e05-47e6-9af4-6684dc10826e)

- Docker Container: Ubuntu 24.04 
![image](https://github.com/kunaljainwin/my-notes/assets/72144717/e3a3a8a1-e1b3-49d7-a37a-48d2ae80b4fa)
![image](https://github.com/kunaljainwin/my-notes/assets/72144717/ebab4bdf-1803-4b6f-81e6-97fbb9ff451f)
- Steps
  1. Install Docker and start docker engine
  2. Docker pull and run container.
- output
  ![image](https://github.com/kunaljainwin/my-notes/assets/72144717/35fad2a8-1d9d-447b-9411-434b54e4b5c4)

### Basis of Time
- Docker reduces time of getting started by 20 times.
- I have myself during this experiment realised the time difference is significant.

# Conclusion

Use docker in these cases:
- Quick hands-on over technologies
- Fast setups and management
- Running Lightweight applications in portable environments

Use VM in these cases:
- Resource isolation
- Resource Intensive needs
- Legacy applications. 
- Complex and critical applications


<h3 style="text-align:center;"> All research for the community ✅ Thank you :)</h3>
