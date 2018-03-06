### Personal Training - ronjay
# Docker
by Docker

---
#### Getting Started
Clone this repository by running :
```shell
$ git clone git@github.com:ronaldjayrjover/dockerLearning.git
$ cd ./docker-labs
```

If you already cloned the lab repo and want to update it with the latest updates / fix to make learning a breeze.  Run the following :
```
$ git pull origin master
```

You may start your laboratory by running :
```bash
$ vagrant up
```

For first time setup, `vagrant` will download the base `vagrant` box used before proceeding setting up the environment.

```bash
Bringing machine ‘puppet’ up with ‘virtualbox’ provider...
Bringing machine ‘master’ up with ‘virtualbox’ provider...
==>  Box ‘centos/7’ could not be found. Attempting to find and install...
...
```

The `vagrant` boxes will be cached to easily spin up new labs when necessary


To check the status of the boxes :
```bash
$ vagrant status
Current machine states:

docker                    poweroff (virtualbox)

This environment represents multiple VMs. The VMs are all listed
above with their current state. For more information about a specific
VM, run `vagrant status NAME`.
```



To access the box, connect via :
```shell
$ vagrant ssh
```

To end sessions :
```shell
$ vagrant halt
```
This will shutdown all VMs


To cleanup the lab :
```shell
$ vagrant destroy
```
This will destroy all VMs

In case one of the lab vms encounter provisioning errors, just run :
```shell
$ vagrant provision
```
To run the provisioning scripts that failed.


---


-
