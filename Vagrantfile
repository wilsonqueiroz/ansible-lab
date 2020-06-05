# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrant Settings
Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.box_check_update = false
  config.vm.network "private_network", ip: "192.168.33.10"
  config.disksize.size = "12GB" # You need install plugin vagrant-disksize on vagrant. For this, do vagrant plugin install vagrant-disksize.

  config.vm.provision "shell", inline: <<-SHELL
    echo "Treinamento Ansible" > /tmp/ansible.txt
  SHELL

  #Virtualbox Settings
  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
    vb.name = "Centos7"
    vb.memory = "1024"
    vb.cpus = "1"
  end
end