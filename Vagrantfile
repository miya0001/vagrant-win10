# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.require_version '>= 1.8'

Vagrant.configure(2) do |config|
  config.vm.box = "Microsoft/EdgeOnWindows10"
  config.vm.box_version = "1.0"
  config.vm.guest = :windows
  config.vm.communicator = "winrm"

  config.winrm.username = "IEUser"
  config.winrm.password = "Passw0rd!"

  config.vm.provider "virtualbox" do |vb|
    vb.name = "win10"
    vb.memory = 4096
    vb.customize ["modifyvm", :id, "--vram", "256"]
    vb.customize ["modifyvm", :id, "--cpus", "2"]
    vb.customize ["modifyvm", :id, "--ioapic", "on"]
    vb.customize ["modifyvm", :id, "--clipboard", "bidirectional"]
    vb.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
    vb.gui = true
  end
end
