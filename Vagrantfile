Vagrant.configure("2") do |config|

  config.vm.define "kali" do |k|
    k.vm.box = "kalilinux/rolling"
    k.vm.hostname = "kali"
    k.vm.network "private_network", ip: "192.168.56.10"

    # Increase memory and CPUs for Kali
    k.vm.provider "virtualbox" do |vb|
      vb.memory = 4096
      vb.cpus = 2
    end
  end

  config.vm.define "ubuntu" do |u|
    u.vm.box = "ubuntu/bionic64"
    u.vm.hostname = "ubuntu"
    u.vm.network "private_network", ip: "192.168.56.11"
    u.vm.boot_timeout = 600

    # You can also configure resources for Ubuntu if needed
    u.vm.provider "virtualbox" do |vb|
      vb.memory = 4096
      vb.cpus = 2
    end
  end

end
