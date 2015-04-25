# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "redis"
    config.vm.box_url = "https://github.com/kraksoft/vagrant-box-ubuntu/releases/download/14.04/ubuntu-14.04-amd64.box"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "site.yml"
    ansible.host_key_checking = false
  end
end
