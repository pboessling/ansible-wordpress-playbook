# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-7.4"

  config.vm.define "app1" do |server|
    server.vm.hostname = "server.example.com"
    server.vm.network :private_network, ip: "192.168.60.4"
  end

  # Run Ansible from the Vagrant VM
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.verbose = true
  end

end
