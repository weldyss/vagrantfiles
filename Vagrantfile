# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant::Config.run do |config|

  config.vm.box = "ubuntuserver"
  config.ssh.username = "ubuntu"
  config.ssh.private_key_path = "/Users/weldyss/.ssh/id_rsa"

  config.vm.define :scoola do |c|
    c.vm.network :bridged
    c.vm.forward_port 22, 2222
  end

  config.vm.define :nwsoft do |c|
    c.vm.network :bridged
    c.vm.forward_port 22, 2223
    c.vm.forward_port 80, 8081
  end
end
