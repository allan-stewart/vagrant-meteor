VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.provision :shell, path: "./bootstrap.sh"
  
  config.vm.network "forwarded_port", guest:3000, host:3000
  
  config.vm.provider "virtualbox" do |v|
    v.memory = 512
    v.cpus = 1
  end
end
