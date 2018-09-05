# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = '2'.freeze
PLAYBOOK = 'configuration-management/ansible/playbook.yml'.freeze

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define 'debian', primary: true do |debian|
    debian.vm.box = 'bento/debian-9.5'

    debian.vm.provision 'ansible' do |ansible|
      ansible.playbook = PLAYBOOK
    end
  end
end
