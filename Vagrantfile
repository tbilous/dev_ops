# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
BOX_IMAGE = "ubuntu/bionic64"

Vagrant.configure("2") do |config|
  config.vm.define "first" do |subconfig|
    subconfig.vm.box = BOX_IMAGE
    subconfig.vm.hostname = "first"
    subconfig.vm.network :private_network, ip: "10.0.0.10"
  end

  config.vm.define "second" do |subconfig|
    subconfig.vm.box = BOX_IMAGE
    subconfig.vm.hostname = "second"
    subconfig.vm.network :private_network, ip: "10.0.0.11"
  end
end
