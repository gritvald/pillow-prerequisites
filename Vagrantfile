# vim: ft=ruby

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.box_url = "https://cloud-images.ubuntu.com/vagrant/trusty/20150609/trusty-server-cloudimg-amd64-vagrant-disk1.box"
  config.vm.box_download_checksum = "dfc2a26686aefe9d55519bc41f504655"
  config.vm.box_download_checksum_type = "md5"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "test.yml"
    ansible.sudo = true
    ansible.host_key_checking = false
  end
end
