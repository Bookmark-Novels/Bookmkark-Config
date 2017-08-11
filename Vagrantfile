# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.provision "shell", inline: <<-SHELL
    wget -O - --quiet https://raw.githubusercontent.com/Bookmark-Novels/Resources/master/Tools/Scripts/vagrant_bootstrap.sh | sh
    pip3 install -r /vagrant/requirements.txt
  SHELL
end