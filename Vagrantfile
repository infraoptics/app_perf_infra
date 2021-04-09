Vagrant.require_version ">= 1.8.0"

Vagrant.configure(2) do |config|

  config.vm.box = "generic/ubuntu2004"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "install.yml"
    ansible.verbose = "v"
    ansible.vault_password_file = "./vault_password"
  end
end
