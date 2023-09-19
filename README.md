# Create-NFS-Server

On this Repo we´ll one way that we can create a NFS Server for Kubernetes NFS storage.

![alt text](https://github.com/DockerSailor/Create-NFS-Server/blob/main/nfs.jpg?raw=true)

First we need to download the ISO file of [TrueNas](https://www.truenas.com/), we can select between CORE or Scale, in this tutorial we´ll be using the CORE edition, you can get it form [here](https://www.truenas.com/truenas-core/).
Once we have the ISO downloaded we start we check the specs for the installation proccess:

- 8 GB Memory
- 16 GB SSD boot device
- 2-Core Intel 64-Bit or AMD x86_64 processor

Now when the system is installed, we log in through web-ui, we can get the server IP on the console logs when we start the server, in my case is [https://192.168.1.36](https://192.168.1.36])
