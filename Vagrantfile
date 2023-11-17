Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/bionic64"
  
  config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.inventory_path = "./hosts"
    ansible.raw_arguments = [
      "--private-key=/home/sardor/ab-haproxy/.vagrant/machines/default/virtualbox/private_key"
]
    ansible.playbook = "playbook.yml"
  end
end
