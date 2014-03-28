Vagrant.configure("2") do |config|
    config.vm.box = "precise32"
    config.vm.box_url = "http://files.vagrantup.com/precise32.box"
    config.vm.network :forwarded_port, guest: 80, host: 8080
    config.vm.synced_folder "www-data/", "/var/www/"
    config.vm.provider "virtualbox" do |machine|
    	machine.memory = 512
    end
    config.vm.provision :shell, path: "provision.sh"
end