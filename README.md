# Create-NFS-Server

On this Repo we´ll one way that we can create a NFS Server for Kubernetes NFS storage.

![alt text](https://github.com/DockerSailor/Create-NFS-Server/blob/main/nfs.jpg?raw=true)

First we need to download the ISO file of [TrueNas](https://www.truenas.com/), we can select between CORE or Scale, in this tutorial we´ll be using the CORE edition, you can get it form [here](https://www.truenas.com/truenas-core/).
Once we have the ISO downloaded we start we check the specs for the installation proccess:

- 8 GB Memory
- 16 GB SSD boot device
- 2-Core Intel 64-Bit or AMD x86_64 processor

Now when the system is installed, we log in through web-ui, we can get the server IP on the console logs when we start the server, in my case is [http://192.168.1.36](http://192.168.1.36]), when we try to log in we need to log with the root user and the password that we set up on the installation menu.

Now we go to the Storage option and then acccess to the Pool submenu:
![alt text](https://github.com/DockerSailor/Create-NFS-Server/blob/main/storage.png?raw=true)

Once there we create a pool:
![alt text](https://github.com/DockerSailor/Create-NFS-Server/blob/main/pool.png?raw=true)

Now we move to the Shell option and move to the `/mnt/our_pool` so we move to `/mnt/NFS_Kubernetes`, then we switch the owner of the folder to ´chown nobody:nogroup /mnt/NFS_Kubernetes´ and give all permisions with ´chmod 777 /mnt/NFS_Kubernetes´:
![alt text](https://github.com/DockerSailor/Create-NFS-Server/blob/main/shell.png?raw=true)
