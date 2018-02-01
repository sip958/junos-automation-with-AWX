# Documentation structure
[**About AWX**](README.md#about-this-project)  
[**About this repo**](README.md#about-this-repo)  
[**How to use this repo**](README.md#how-to-use-this-repo)  

# About AWX

AWX is Ansible Tower open sourced.  
You can it if you want to consume your ansible playbooks with:
- GUI
- REST API
- users authentication and permissions. 

Here's the [**AWX FAQ**](https://www.ansible.com/products/awx-project/faq)  
Here's the [**AWX REST API guide**](http://docs.ansible.com/ansible-tower/2.3.0/html/towerapi/index.html)  
You can visit the AWX REST API with a web browser: http://<AWX_IP_ADDRESS>/api/v2/  

# About this repo  

This repository has automation content that configure AWX. If you want to use AWX to consume playbooks, you can use this repository to quickly add them to AWX.  
This repository has automation content that consume AWX (execute playbooks with REST calls).    
It uses Python scripts and YAML variables. The python scripts use the library **requests** to makes REST calls to AWX.   

# How to use this repo 
You need to: 
- install AWX
- install Ansible requirements for Junos
- clone this repository
- edit the file [variables.]

# install AWX

# install the Ansible requirements for Junos

## install the python library **requests**
```
sudo -s
pip install requests
```
## clone the repository and move to the local directory
```
sudo -s
git clone https://github.com/ksator/junos-automation-with-AWX.git
cd junos-automation-with-AWX
```

The file [**variable.yml**](variable.yml) has variables. You need to edit it to indicates details such as: 
- The IP address of your AWX  
- 


```
vi variable.yml
```
```
# python configure_awx_from_variables.py 
Juniper organization successfully created
automation team successfully created and added to the Juniper organization
ksator user successfully created and added to the automation team
Junos automation project successfully created and added to the Juniper organization
junos credentials successfully created and added to the Juniper organization
junos_lab inventory successfully created and added to the Juniper organ
hosts file successfully added as a source to junos_lab inventory
wait 20 seconds before to resume
pb.check.lldp.yml template successfully created
pb.check.bgp.yml template successfully created
pb.check.interfaces.yml template successfully created
pb.check.vlans.yml template successfully created
pb.check.lldp.json.yml template successfully created
pb.configure.golden.yml template successfully created
pb.configure.telemetry.yml template successfully created
pb.rollback.yml template successfully created
pb.print.facts.yml template successfully created
pb.check.all.yml template successfully created
pb.check.ports.availability.yml template successfully created
```
# Looking for more Junos automation solutions

https://github.com/ksator?tab=repositories  
https://gitlab.com/users/ksator/projects  
https://gist.github.com/ksator/  

