# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "scotch/box"
    config.vm.network "private_network", ip: "192.168.33.10"
    config.vm.hostname = "scotchbox"

    config.vm.synced_folder "public", "/var/www", :mount_options => ["dmode=777", "fmode=666"]
    config.vm.synced_folder "shared", "/home/vagrant/shared", :mount_options => ["dmode=777", "fmode=666"]
end
