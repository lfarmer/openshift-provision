Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.hostname = "openshift-local"
  config.vm.network "forwarded_port", guest: 8443, host: 8443, auto_correct: true

  config.vm.provider :virtualbox do |v|
    v.customize ["modifyvm", :id, "--memory", 2048]

  end

  config.vm.network "private_network", ip: "192.168.33.10"

end
