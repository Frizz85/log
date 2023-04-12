# -*- mode: ruby -*- 
# vi: set ft=ruby : 
Vagrant.configure(2) do |config| 
  config.vm.box = "centos/7" 
  config.vm.box_version = "2004.01" 
  config.vm.provider "virtualbox" do |v| 
  v.memory = 512 
  v.cpus = 1 
 end 
 config.vm.define "web" do |web| 
  web.vm.network "public_network", ip: "192.168.50.10" 
#,  virtualbox__intnet: "net1" 
  web.vm.hostname = "web"
 end 
 config.vm.define "log" do |log| 
  log.vm.network "public_network", ip: "192.168.50.11" 
#,  virtualbox__intnet: "net1" 
  log.vm.hostname = "log"
 end 
end
