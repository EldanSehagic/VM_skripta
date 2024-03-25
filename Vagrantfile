
Vagrant.configure("2") do |config|
 
 config.vm.box = "ubuntu/focal64"

config.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
      vb.cpus = 2
end

config.vm.network "private_network", ip:"192.168.33.10"

config.vm.provision "shell", inline: <<-SHELL
  sudo apt-get update
  sudo apt-get install -y git
SHELL

end