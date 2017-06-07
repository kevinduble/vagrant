# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
   config.vm.provider "virtualbox" do |vb|
#     Uncomment if you need the VirtualBox VM console
#     vb.gui = true
     vb.memory = "1024"
   end
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "VM.yml"
  end
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.network "forwarded_port", guest: 443, host: 8443
end
