# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.provider "virtualbox" do |vb|
    vb.memory = 2048
    vb.cpus = 2
  end

  config.vm.provider "vmware_desktop" do |v|
    v.vmx["memsize"] = "2048"
    v.vmx["numvcpus"] = "2"
  end

  config.vm.box = "ubuntu/focal64"
  config.vm.define "grafana"
  config.vm.network "forwarded_port", guest: 3000, host: 3000

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "./provisioning/main.yml"
  end
end
