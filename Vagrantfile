# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"

  # config.vm.network "forwarded_port", guest: 80, host: 8080

  # Create a private network, which allows host-only access to the machine
  config.vm.network "private_network", ip: "192.168.33.1"

  # If true, then any SSH connections made will enable agent forwarding.
  config.ssh.forward_agent = true

  # config.vm.synced_folder "../data", "/vagrant_data"

  config.vm.provider "virtualbox" do |vb|
    vb.name = "sandbox"
    vb.gui = false
    vb.memory = "1024"
  end
end
