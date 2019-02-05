Vagrant.configure("2") do |config|
  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "generic/ubuntu1804"
    ubuntu.vm.synced_folder '.', '/vagrant', disabled: true
    ubuntu.vm.provider :libvirt do |domain|
      domain.memory = 4096
      domain.cpus = 2
    end
  end
end
