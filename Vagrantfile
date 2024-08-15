# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  # https://docs.vagrantup.com.

  # boxes at https://vagrantcloud.com/search.
  config.vm.define "wordpress" do |wordpress|
    wordpress.vm.hostname = "wordpress.local"
    wordpress.vm.box = "alvistack/ubuntu-24.04"
    wordpress.vm.network "private_network", ip: "192.168.56.10"
  end

  config.vm.define "db" do |db|
    db.vm.hostname = "db.local"
    db.vm.box = "alvistack/ubuntu-24.04"
    db.vm.network "private_network", ip: "192.168.56.20"
  end
  
  # config.vm.provider "virtualbox" do |vb|
  #   # Display the VirtualBox GUI when booting the machine
  #   vb.gui = true
  #
  #   # Customize the amount of memory on the VM:
  #   vb.memory = "1024"
  # end

  # Enable provisioning with a shell script. Additional provisioners such as
  # Ansible, Chef, Docker, Puppet and Salt are also available. Please see the
  # documentation for more information about their specific syntax and use.
  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL
end
