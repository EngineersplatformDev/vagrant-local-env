vagrant.configure("2") do |config|:

#Ubuntu virtual machine. Can be used for installing any web server. 
	config.vm.define "web" do |web|:
		web.vm.box = "ubuntu/xenial64"
		web.vm.provision "shell", inline: <<-SHELL
			echo "hello this is my first project file! I proclaim my Lord JESUS is my Savior!"
		SHELL
	end

#CentOS VM. Can be used for installing application server 
	config.vm.define "webapp" do |webapp|:
		webapp.vm.box = "centos/7"
		webapp.vm.provision "shell", inline: <<-SHELL
			echo "this vm is for centos OS. I keep going up in the mighty name of JESUS!"
		SHELL
	end
end