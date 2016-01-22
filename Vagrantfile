Vagrant.configure(2) do |config|
  config.vm.box = "nrel/CentOS-6.5-x86_64"
  config.vm.provision :shell, path: "bootstrap.sh"
  config.vm.network "public_network", ip: "192.168.1.199"
end
