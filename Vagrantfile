Vagrant.configure("2") do |config|
  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "generic/ubuntu1910"
    ubuntu.vm.synced_folder '.', '/vagrant', disabled: true
    ubuntu.vm.network :forwarded_port, guest: 8888, host: 8888
    ubuntu.vm.provider :libvirt do |domain|
      domain.memory = 4096
      domain.cpus = 2
    end
  end
end
