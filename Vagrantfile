Vagrant.configure("2") do |config|
  config.vm.define "VM1" do |debup|
    debup.vm.box = "debian/bookworm64"
    debup.vm.synced_folder "./", "/vagrant"
    debup.vm.hostname = "deb12"
    debup.vm.boot_timeout = 450
    debup.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
      vb.cpus = "2"
    end
  end
end
