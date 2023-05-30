Vagrant.configure(2) do |config|
	config.vm.box = "centos/7"
	config.vm.network "public_network"
	(1..3).each do |i|
		config.vm.define "vm#{i}" do |node|
			config.vm.provider "virtualbox" do |node|
				node.name = "vm#{i}"  
			end
		end
	end
end
