# -*- mode: ruby -*-
# vi: set ft=ruby :
# See README.md for details

#VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(2) do |config|

  config.vm.define "master"  do |ctl|
    ctl.vm.synced_folder '.', '/vagrant', disabled: true
    ctl.vm.box = "centos/7"
        ctl.vm.hostname = "master"
        ctl.vm.network "private_network", ip: "172.31.0.10"
        ctl.vm.provider "virtualbox" do |vb|
          vb.memory = 2048
        end
  end
end
