Vagrant.configure("2") do |config|
  config.vm.box = "boxomatic/centos-stream-9"
  config.vm.hostname = 'sonarqueb'
  config.vm.network 'forwarded_port', guest: 9000, host: 9000, hostip: '127.0.0.1'
  config.vm.provision 'shell', path: 'provision.sh'
  config.vm.provider 'virtualbox' do |v|
    v.memory = 2048
  end
end
