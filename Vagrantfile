# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.require_version '>= 1.8'

Vagrant.configure(2) do |config|
  config.vm.box = "modernIE/w10-edge"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = 2048
    vb.customize ["modifyvm", :id, "--vram", "256", "--cpus", "2", "--ioapic", "on"]
    vb.gui = true
  end
end
