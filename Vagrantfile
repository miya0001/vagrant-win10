# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "modernIE/w10-edge"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = 2048
    vb.customize [ "modifyvm", :id, "--vram", "128" ]
    vb.gui = true
    vb.linked_clone = true
  end
end
