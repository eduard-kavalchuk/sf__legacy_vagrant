Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  config.vm.box_check_update = false

  config.vm.provision "shell", inline: <<-SHELL
    apt update
    apt install -y postgresql postgresql-contrib
	systemctl start postgresql.service
  SHELL
end
