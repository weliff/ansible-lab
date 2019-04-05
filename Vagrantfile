Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/trusty64"

    config.vm.provider "virtualbox" do |virtualbox|
        virtualbox.memory = 1024
    end

    config.vm.define "wordpress" do |wordpress|
        wordpress.vm.network "private_network", ip: "172.17.177.40"
    end

    config.vm.define "mysql" do |mysql|
        mysql.vm.network "private_network", ip: "172.17.177.41"
    end
end
