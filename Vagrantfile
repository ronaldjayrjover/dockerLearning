# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

    config.vm.box = "centos/7"

    config.vm.define "docker" do |docker|
        docker.vm.hostname = "docker.ronjay"


        docker.vm.provision "shell",
            path: "scripts.d/init.d/docker"

        docker.vm.network "private_network", ip: "192.168.200.22"

        docker.vm.provider :virtualbox do |vb|
            vb.name = "docker.ronjay"
        end
    end

end
