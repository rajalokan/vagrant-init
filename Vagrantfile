# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.hostname = "playbox"
  config.vm.box_check_update = false

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "bootstrap.yml"
    # ansible.tags = ["bash"]
    # ansible.verbose = true
    # ansible.extra_vars = { "deployment_type": "vagrant", "deployments": [] }
    ansible.galaxy_roles_path = "~/playground/rajalokan/ansible_roles"
  end
end
