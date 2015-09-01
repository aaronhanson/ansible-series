# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.provider "virtualbox" do |vbox|
    vbox.customize ["modifyvm", :id, "--memory", "1024"]
  end

  config.vm.define "web0" do |web0|
    web0.vm.network "private_network", ip: "192.168.10.10"
  end

  config.vm.define "db0" do |db0|
    db0.vm.network "private_network", ip: "192.168.10.20"
  end
end
