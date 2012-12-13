# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant::Config.run do |config|
    config.vm.box = "precise64"
    config.vm.box_url = "http://files.vagrantup.com/precise64.box"

  config.vm.provision :puppet do |puppet|
  	puppet.manifests_path = "."
    puppet.manifest_file = "vagrant.pp"
    puppet.module_path = "../"
  end
 		 
  config.vm.forward_port 80, 4567
end