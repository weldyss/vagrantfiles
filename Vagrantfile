# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant::Config.run do |config|

  config.vm.box = "ubuntuserver"
  config.ssh.username = "ubuntu"
  config.ssh.private_key_path = "/Users/weldyss/.ssh/id_rsa"

  config.vm.define :scoola do |local_config|
    local_config.vm.network :hostonly, "10.55.55.10"
    local_config.vm.forward_port 22, 2222
  end

  config.vm.define :nwsoft do |local_config|
    local_config.vm.network :hostonly, "10.55.55.11"
    local_config.vm.forward_port 22, 2223
    local_config.vm.forward_port 80, 8081
  end
end
