Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.provision :shell, path: "setup.sh"
  config.vm.synced_folder ".", "/var/www/app"
  config.vm.network "forwarded_port", guest: 3000, host: 3000
end
