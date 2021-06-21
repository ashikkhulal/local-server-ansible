Vagrant.configure("2") do |config|
  config.hostmanager.enabled = true 
  config.hostmanager.manage_host = true
  
### Master ###
  config.vm.define "master" do |master|
    master.vm.box = "ubuntu/xenial64"
    master.vm.hostname = "master"
	  master.vm.network "private_network", ip: "192.168.33.10"
        master.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      end
  end

### Node 1 ###
  config.vm.define "server01" do |server01|
    server01.vm.box = "ubuntu/xenial64"
    server01.vm.hostname = "server01"
    server01.vm.network "private_network", ip: "192.168.33.11"
        server01.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      end
  end
end