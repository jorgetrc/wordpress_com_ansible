Vagrant.configure("2") do |config|

    config.vm.box = "ubuntu/jammy64"

    config.vm.provider "virtualbox" do |v|
        v.memory = 1024
    end

    config.vm.define "wordpress" do |m|
        m.vm.network "public_network", ip: "192.168.15.20", bridge: "enp5s0"
    end

    config.vm.define "mysql" do |m|
        m.vm.network "public_network", ip: "192.168.15.21", bridge: "enp5s0"
    end
end
