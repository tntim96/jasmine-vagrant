Vagrant.configure("2") do |config|
  config.vm.box = "debian80"
  config.vm.box_url = "debian80.box"
  config.vm.network :forwarded_port, guest: 80, host: 80
  config.vm.network :forwarded_port, guest: 8888, host: 8888
  config.vm.network :private_network, ip: "192.168.33.10"
  config.vm.synced_folder "c:/js", "/vagrant_js"
end
