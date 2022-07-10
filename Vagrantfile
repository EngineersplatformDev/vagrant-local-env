Vagrant.configure("2") do |config|
	config.hostmanager.enabled = true
	config.hostmanager.manage_host = true

#Ubuntu virtual machine. Can be used for installing any web server. 
	config.vm.define "web" do |web01|
		web01.vm.box = "ubuntu/xenial64"
		web01.vm.hostname = "web01"
		web01.vm.network "private_network", ip: 192.168.56.11
		web01.vm.provision "shell", inline: <<-SHELL
			echo "hello this is my first project file! I proclaim my Lord JESUS is my Savior!"
		SHELL
	end

#CentOS VM. Can be used for installing application server 
	config.vm.define "app01" do |app01|
		app01.vm.box = "centos/7"
		app01.vm.hostname = "app01"
		app01.vm.network "private_network", ip: 192.168.56.12
		app01.vm.provision "shell", inline: <<-SHELL
			echo "this vm is for centos OS. I keep going up in the mighty name of JESUS!"
		SHELL
	end

#memcache vm 
	config.vm.define "mc01" do |mc01|
		mc01.vm.box = "centos/7"
		mc01.vm.hostname = "mc01"
		mc01.vm.network "private_network", ip: 192.168.56.14
		mc01.vm.provision "shell", inline: <<-SHELL
			echo "this vm is for centos OS. I keep going up in the mighty name of JESUS!"
		SHELL
	end

##Rabbit MQ
	config.vm.define "rmq01" do |rmq01|
		rmq01.vm.box = "centos/7"
		rmq01.vm.hostname = "rmq01"
		rmq01.vm.network "private_network", ip: 192.168.56.16
		rmq01.vm.provision "shell", inline: <<-SHELL
			echo "this vm is for centos OS. I keep going up in the mighty name of JESUS!"
		SHELL
	end


	config.vm.define "db01" do |db01|
		db01.vm.box = "centos/7"
		db01.vm.hostname = "db01"
		db01.vm.network "private_network", ip: 192.168.56.15
		db01.vm.provision "shell", inline: <<-SHELL
			echo "this vm is for centos OS. I keep going up in the mighty name of JESUS!"
		SHELL
	end
end