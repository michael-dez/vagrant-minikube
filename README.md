> This is a fork of mintel/vagrant-minikube which does not appear to be maintained. The sshfs and libvirt plugins were removed for better Windows compatibility. The Kubernetes version environment variable has also been updated to 1.23.3 and the conntrack package has been added to the main startup script.
# Minikube Vagrant

Provide a consistent way to run minikube locally across different distro's..
Note, this installs `minikube` and `kubectl` for ubuntu 16.04.

## Install Pre-requisites
### Vagrant

Ensure you have vagrant installed (should also support mac/windows)

* [Installation/Download](https://www.vagrantup.com/docs/installation/)

#### Using Arch Package Manager
```
sudo pacman -S vagrant
```

#### Using Ubuntu Package Manager
```
sudo apt-get install vagrant
```
### VirtualBox
* [Installation](https://www.virtualbox.org/manual/ch02.html)
* [Download Page](https://www.virtualbox.org/wiki/Downloads)


## Run it

Clone and enter this repo, then:

```
vagrant up
```

## SSH into the VM
```
vagrant ssh
```

## Check minikube is up and running

```
kubectl get nodes
```

