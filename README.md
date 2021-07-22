# Vagrant-start-k8s

**This project provides a quick way to start kubernets nodes** 

## Pre-requisites

1. [Install VirtualBox](https://www.virtualbox.org/wiki/Downloads)
2. [Install Vagrant](https://www.vagrantup.com/downloads)

## QuickStart

```Bash
1. git clone https://github.com/DeyunLuo/vagrant-start-k8s.git
2. cd vagrant-start-k8s/k8s_vagrant
3. vagrant up
4. vagrant ssh default
5. kubeadm init --pod-network-cidr=10.244.0.0/16
```



