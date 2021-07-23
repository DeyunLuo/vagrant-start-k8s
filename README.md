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
6. sudo su  
7. # If you have worker node want to join master Please input prestep print like this
 # kubeadm join 10.0.2.15:6443 --token 9s57cv.0plnulaw1auw0qc3 --discovery-token-ca-cert-hash sha256:850ca59741aa91eed92955caa77c35dd7a5da7a3d6d40fe1a4b81d8ba69dea85
```

## Install Flannel Network Cni
```bash
kubectl apply -f https://raw.githubusercontent.com/coreos/flannel/master/Documentation/kube-flannel.yml
```



