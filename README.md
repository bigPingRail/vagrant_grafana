### Description:  
Simple ubuntu 20.04 virtual machine with docker and minimal grafana stack on board with pre installed Node Exporter dashboard which provide basic vm performance metrics  
#### Requirements:  
[Hashicorp vagrant](https://www.vagrantup.com/downloads)  
[Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)  
[VMware player](https://customer connect.vmware.com/en/downloads/details?downloadGroup=WKST-PLAYER-1623-NEW&product Id=1039&rPId=85399)  
#### Build and run:  
Download repo, and `cd` into it and run `vagrant up`  
When all things is done you can able to log in to grafana default page, which is reachable by default at `http//localhost:3000`  
Anonymous access is enabled, also you can login to grafana via Admin credentials  
by default creds are   
Username = `Admin`  
Password = `testpass`  