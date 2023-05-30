Vagrant.configure(2) do |config|
	# Specifying the box we wish to use
	config.vm.box = "chef/centos-6.5"
	# Adding Bridged Network Adapter
	config.vm.network "public_network"
	# Iterating the loop for three times
	(1..3).each do |i|
		# Defining VM properties
		config.vm.define "vm#{i}" do |node|
			# Specifying the provider as VirtualBox and naming the VM's
			config.vm.provider "virtualbox" do |node|
				# The VM will be named as edureka_vm{i}
				node.name = "vm#{i}"  
			end
		end
	end
end
