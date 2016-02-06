Vagrant.configure(2) do |config|

  # Setup Ubuntu Trusty64 14.04 Box.
  config.vm.define "trusty", primary: true do |trusty|
    trusty.vm.box = "ubuntu/trusty64"
  end

  # Setup Ubuntu Precise64 14.04 Box.
  config.vm.define "precise" do |precise|
    precise.vm.box = "ubuntu/precise64"
  end

  # Setup CentOS 7 Box.
  config.vm.define "centos7" do |centos7|
    centos7.vm.box = "centos/7"
  end

  # Enable ansible as the provisioner.
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "tasks/main.yml"
  end

end
