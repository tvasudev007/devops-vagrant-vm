# Devops tool kit setup using vagrant

This reposiroty is intended to setup a quick devops tool kit using vagrant.

The following tools are installed in the vm:
1. Terraform
2. Python
3. Ansible
4. Docker
5. Kubectl
6. Git

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

The following softwares should already be installed to setup vm using vagrant

* [Virtualbox](https://www.virtualbox.org/wiki/Downloads) - VirtualBox is a general-purpose full virtualizer
* [Vagrant]( https://www.vagrantup.com/downloads.html) - Vagrant is a tool for building and managing virtual machine environments in a single workflow
* Vagrantfile expects folder "Users/Interview" to be present on the host machine


### Getting started

data can be synced between host & guest m/c by placing data in the following path:
```
HOST_PATH: /users/Interview & GUEST_PATH: / home/ devops-vm/ devops-vm
```

To start a box/vm, use the following
```
vagrant up
```
To access the vm

```
vagrant ssh
```
To save the current running state of the machine and stop it.
```
vagrant suspend
```
To save the current running state of the machine and stop it.
```
vagrant suspend
```
To gracefully shut down the guest operating system and power down the guest machine
```
vagrant halt
```
To remove all traces of the guest machine from your system. It'll stop the guest machine, power it down, and remove all of the guest hard disks
```
vagrant destroy
```
To remove all boxes that may have been installed on your computer during "vagrant up"
```
vagrant box remove -f ubuntu/trusty64
```
To forcifully destory all the instances
```
vagrant destroy -f --[no-]parallel 
```

## Additional resources

Add additional notes about vagrant can be found at: https://www.vagrantup.com/docs/index.html


## License

This project is licensed under the GNU GENERAL PUBLIC LICENSE - see the [LICENSE](LICENSE) file for details


