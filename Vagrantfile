# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Config for the first VM based on Ubuntu.
  config.vm.define "Ubuntu-1" do |ub1|
    ub1.vm.box = "ubuntu/xenial64"
    ub1.vm.hostname = "Ubuntu-1"
 
    ub1.vm.provider "virtualbox" do |vb|
      # Display the VirtualBox GUI when booting the machine
      vb.gui = false
  
      # Customize the amount of memory on the VM:
      vb.memory = "512"
    end
  end

  # Config for the second VM based on CentOS.
  config.vm.define "CentOS-1" do |cent1|
    cent1.vm.box = "centos/7"
    cent1.vm.hostname = "CentOS-1"

    cent1.vm.provider "virtualbox" do |vb|
      # Display the VirtualBox GUI when booting the machine
      vb.gui = false
  
      # Customize the amount of memory on the VM:
      vb.memory = "512"
    end
  end

end
