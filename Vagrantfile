# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|    
  config.vm.define "kurseve" do |server|
    server.vm.box = "ubuntu/trusty64"
    server.vm.hostname = "kurseve"
    server.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
      vb.cpus = "2" 
    end
    server.ssh.insert_key = false
    server.vm.provision "ansible" do |ansible|
      ansible.verbose = "-vvv"
      # If you want a less verbose one. Uncomment this.
      # ansible.verbose = "-v"
      ansible.playbook = "playbook.yml"
    end
  end
end
