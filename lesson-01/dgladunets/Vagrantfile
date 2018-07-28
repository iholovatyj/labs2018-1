# (C) Dima Gladunets 2018
# Lesson 1

Vagrant.configure("2") do |config|

    config.vm.define "ubuntu1" do |ubuntu1|
    ubuntu1.vm.box = "ubuntu/xenial64"
    ubuntu1.vm.hostname = 'ubuntu1'
    ubuntu1.vm.box_url = "ubuntu/xenial64"

    ubuntu1.vm.network :forwarded_port, guest: 22, host: 8082, id: "ssh"
    
   
   	
      ubuntu1.vm.provider :virtualbox do |v|
      v.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
      v.customize ["modifyvm", :id, "--memory", 512]
      v.customize ["modifyvm", :id, "--name", "ubuntuEPAMLAB"]
    end
  end

    config.vm.define "centos7" do |centos7|
    centos7.vm.box = "centos/7"
    centos7.vm.hostname = 'centos7'
    centos7.vm.box_url = "centos7"

    centos7.vm.network :forwarded_port, guest: 22, host: 8083, id: "ssh"
    	
    
      centos7.vm.provider :virtualbox do |v|
      v.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
      v.customize ["modifyvm", :id, "--memory", 512]
      v.customize ["modifyvm", :id, "--name", "centos7EPAMLAB"]
    end
  end

end

