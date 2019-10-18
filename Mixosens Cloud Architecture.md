# Mixosens Cloud Architecture

## Server Cluster TC

### Ubuntu Server [ 192.168.1.5 ] 

- Jenkins 
- Docker Container
- BitBucket
- Netdata Monitor
- FTP Server -> Port: 21

	- FTP访问资源说明

		- /home/<Account>/<Resources>
		- /home/mixo_sw_server/mnt/AzureBackupDisk
		- /home/mixo_sw_server/mnt/ds218
		- /home/mixo_sw_server/mnt/ds918

- SSH -> Port:4444
- Rsync

	- NAS

		- DS218 - 192.168.1.7:8001 /shared01 -> /home/mixo_sw_server/mnt/ds218
		- DS918 - 192.168.1.8:5000 /shared01 -> /home/mixo_sw_server/mnt/ds218
		- Azure AIgo VM: 139.217.132.198:/data -> /home/mixo_sw_server/mnt/AzureBackupDisk 

### Windows Server [ 192.168.1.6 ]

- Jenkins
- CMake
- Team Viewer

### Redhat Server [ 192.168.1.4 ]

- Simulator
- VMware 

	- EDA

- Report

	- Sublime、LibreOffice

- VNC
- Samba
- FTP Server -> Port:21
- SSH -> Port: 22

## Azure Cloud CN

### AIgo VM [ 139.217.132.198 ]

- Jupyter Notebook
- Jupyter Lab
- Jupyterhub
- Docker Container
- miniconda
- cmake
- git
- Rsync
- Data
- LAMP Env
- FTP Internal

	- FTP Resources

		- /data
		- /home/<Account>/<Resources>
		- /home/Common | Public Shared Directory

###  40.73.114.84

- FTP External
- Shared for Forign Guest And Supplier

## Aliyun Cloud

### 106.15.235.141

- 公司官方网站
- Docker Container 
- LAMP Server
- Nginx Reflection

*XMind: ZEN - Trial Version*