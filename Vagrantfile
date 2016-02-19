Vagrant.configure(2) do |config|
  config.vm.network "forwarded_port", guest: 80, host: 8080
    config.vm.box = "ubuntu14.04x64"
    config.vm.box_url = "https://oss-binaries.phusionpassenger.com/vagrant/boxes/latest/ubuntu-14.04-amd64-vbox.box"
    config.vm.box_url = "./ubuntu-14.04-amd64-vbox.box"
    config.vm.network "private_network", ip: "10.0.1.290"
    
    config.vm.provision :ansible do |ansible|
     ansible.playbook = "playbook.yml"
  end
end
