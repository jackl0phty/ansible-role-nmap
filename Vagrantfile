Vagrant.configure(2) do |config|

  # Setup Ubuntu Trusty64 14.04 Box.
  config.vm.box = "ubuntu/trusty64"

  # Enable ansible as the provisioner.
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "tasks/main.yml"
  end

end
