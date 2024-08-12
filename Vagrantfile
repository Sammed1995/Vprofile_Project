Vagrant.configure("2") do |config|
    config.hostmanager.enabled = true
    config.hostmanager.manage_host = true

    ### DB VM ###
    config.vm.define "db01" do |db01|
      db01.vm.box = "eurolinux-vagrant/centos-stream-9"
      db01.vm.hostname = "db01"
      db01.vm.network "private_network", ip: "192.168.56.61"
      db01.vm.provider "virtualbox" do |vb|
       vb.memory = "600"  
      end 

    end
    
    ### Memcache ###
     config.vm.define "mc01" do |mc01|
      mc01.vm.box = "eurolinux-vagrant/centos-stream-9"
      mc01.vm.hostname = "mc01"
      mc01.vm.network "private_network", ip: "192.168.56.62"
      mc01.vm.provider "virtualbox" do |vb|
       vb.memory = "600"  
      end 
    end
  
     ### RabbitMQ ###
     config.vm.define "rm01" do |rm01|
      rm01.vm.box = "eurolinux-vagrant/centos-stream-9"
      rm01.vm.hostname = "rm01"
      rm01.vm.network "private_network", ip: "192.168.56.63"
      rm01.vm.provider "virtualbox" do |vb|
       vb.memory = "600"  
      end 
    end

     ### tomcat ###
     config.vm.define "app01" do |app01|
      app01.vm.box = "eurolinux-vagrant/centos-stream-9"
      app01.vm.hostname = "app01"
      app01.vm.network "private_network", ip: "192.168.56.64"
      app01.vm.provider "virtualbox" do |vb|
       vb.memory = "600"  
      end 
    end

     ### Nginx ###
     config.vm.define "web01" do |web01||
      web01.vm.box = "ubuntu/jammy64"
      web01.vm.hostname = "web01"
      web01.vm.network "private_network", ip: "192.168.56.65"
      web01.vm.provider "virtualbox" do |vb|
       vb.gui = true
       vb.memory = "600"  
      end
    end
    
  end  
  
