Vagrant.configure("2") do |config|

  # Setup Debian Jessie 64
  config.vm.define "jessie" do |jessie|
    config.vm.box = "debian/jessie64"
  end
  
  # Setup Debian Wheezy 64
  config.vm.define "wheezy" do |wheezy|
    config.vm.box = "debian/wheezy64"
  end
  
  # Setup Ubuntu Trusty 64 14.04 Box.
  config.vm.define "trusty" do |trusty|
    trusty.vm.box = "ubuntu/trusty64"
  end

  # Setup Ubuntu Precise 64 12.04 Box.
  config.vm.define "precise" do |precise|
    precise.vm.box = "ubuntu/precise64"
  end


  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
    vb.memory = "2048"
  end

  config.ssh.insert_key = false

  config.vm.provision "ansible" do |ansible|
    ansible.verbose = "vvvv"
    ansible.playbook = "tests/test.yml"
  end
end


