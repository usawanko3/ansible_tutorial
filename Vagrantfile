# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  # Use centos 6.7
  config.vm.box = 'puphpet/centos65-x64'

  # Contorl machine
  config.vm.define 'control-machine' do |cm|
    cm.vm.hostname = 'control-machine'
    cm.vm.network :private_network, ip: '192.168.33.10'
  end

  # Managed nodes
  config.vm.define 'managed-node-1' do |mn1|
    mn1.vm.hostname = 'managed-node-1'
    mn1.vm.network :private_network, ip: '192.168.33.11'
  end
end
