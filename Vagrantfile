Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "1024"
  end

  config.vm.define "wordpress" do |wordpress|
    wordpress.vm.network "private_network", 
      ip: "192.168.56.7"
  end

  config.vm.define "mysql" do |mysql|
    mysql.vm.network "private_network", 
      ip: "192.168.56.9"
  end
end
