# -*- mode: ruby -*-
# vi: set ft=ruby :
# single vm box. Using rocky linux 9

Vagrant.configure("2") do |config|
  config.ssh.username = "root"
  config.ssh.password = "passwd"
  config.ssh.private_key_path = "C:\\Projects\\rocky9\\.ssh\\id_rsa"
  config.ssh.forward_agent = "true"

  config.vm.define "rocky" do |rocky|
    config.vm.box = "rocky9"
    config.vm.network "public_network", type: "dhcp"

    config.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = "2"
    end
  end

    config.vm.provision "shell", inline: <<-SHELL
      sudo yum update -y
    SHELL
end
