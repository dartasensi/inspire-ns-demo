# -*- mode: ruby -*-
# vi: set ft=ruby :

# #####
# configuration variables
# #####
$_vg_provision_utils_path = './vg-docker/.vg-provision/bootstrap_ubuntu_utils.sh'
$_vg_provision_docker_path = './vg-docker/.vg-provision/bootstrap_ubuntu_docker.sh'

# load Vagrant VM defaults
_vg_defaults_vagrantfile = './vg-docker/Vagrantfile'
load _vg_defaults_vagrantfile if File.exists?(_vg_defaults_vagrantfile)


Vagrant.configure("2") do |config|
  config.vm.define "main", primary: true do |main|
    # only for debug purposes
    main.vm.network "forwarded_port", host: 18081, guest: 8081, auto_correct: true
    main.vm.network "forwarded_port", host: 18082, guest: 8082, auto_correct: true
    main.vm.network "forwarded_port", host: 18083, guest: 8083, auto_correct: true
    main.vm.network "forwarded_port", host: 18084, guest: 8084, auto_correct: true
    main.vm.network "forwarded_port", host: 18085, guest: 8085, auto_correct: true
    main.vm.network "forwarded_port", host: 18086, guest: 8086, auto_correct: true
  end
end