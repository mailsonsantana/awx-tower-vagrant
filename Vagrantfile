Vagrant.configure("2") do |config|

  config.vm.define "database" do |m|
    m.vm.network "public_network", ip: "192.168.0.110"
    config.vm.box = "centos/7"
    config.vm.provider "virtualbox" do |vb|
      #   # Display the VirtualBox GUI when booting the machine
         vb.gui = true
      #
      #   # Customize the amount of memory on the VM:
         vb.memory = "1024"
       end


       
  end
  config.vm.define "ansibleserver" do |m|
    m.vm.network "public_network", ip: "192.168.0.112"
    m.vm.box = "ubuntu/focal64"
    config.vm.provider "virtualbox" do |vb|
      #   # Display the VirtualBox GUI when booting the machine
         vb.gui = true
      #
      #   # Customize the amount of memory on the VM:
         vb.memory = "2048"
       end
  end
end
