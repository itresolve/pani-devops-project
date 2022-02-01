## DEFINITION
Vagrant is just a tool used to easily build and manage VM environments.


#### Create a VM with vagrant
CD to your vagrant directory, then run below cmd to create vagrantfile
```
vagrant init centos/7   # To create vagrantfile
vagrant up   # To build VM
vagrant ssh    # To access VM
```

### FIX

If vagrant fail to build, run bellow cmd and RESTART LAPTOP:
```
bcdedit /copy "{current}" /d "Hyper-V" 
bcdedit /set "{current}" hypervisorlaunchtype off
bcdedit /set "{current}" description "non Hyper-V"
```
OR
Turn ON Hyper-V in Windows features and restart laptop


#### Create Vagranfile mannually
See bellow file

![More here](https://github.com/itresolve/pani-devops-project/blob/prereqs/vagrant1.PNG)



## Vagrant cloud 
Find OS images to this link: 
[More here](https://app.vagrantup.com/boxes/search)

