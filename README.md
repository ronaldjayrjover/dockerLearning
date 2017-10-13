## OpsWerks
training exercises
# Docker
by Docker

---
#### Getting Started
Clone this repository by running :
```shell
$ git clone git@gitlab.com:opswerks/docker-labs.git
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
==> puppet: Box ‘research/xenial16x64’ could not be found. Attempting to find and install...
   puppet: Box Provider: virtualbox
   puppet: Box Version: >= 0
==> puppet: Loading metadata for box ‘research/xenial16x64’
   puppet: URL: https://atlas.hashicorp.com/research/xenial16x64
==> puppet: Adding box ‘research/xenial16x64’ (v0.1.1) for provider: virtualbox
   puppet: Downloading: https://atlas.hashicorp.com/research/boxes/xenial16x64/versions/0.1.1/providers/virtualbox.box
   puppet: Progress: 21% (Rate: 374k/s, Estimated time remaining: 0:24:08)
...
```

The `vagrant` boxes will be cached to easily spin up new labs when necessary

```bash
$ vagrant box list
ansible/tower        (virtualbox, 3.0.2)
centos7x64           (virtualbox, 0)
laravel/homestead    (virtualbox, 0.5.0)
research/centos7x64  (virtualbox, 0.1.1)
research/xenial16x64 (virtualbox, 0.1.1)
```

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

For comments and suggestions, contact us via :email: :
* obie@opswerks.com
* tom@opswerks.com

-
