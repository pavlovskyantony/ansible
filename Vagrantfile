Vagrant.configure("2") do |config|
  config.vm.define "ansblDay1H" do |ansblDay1h|
  ansblDay1h.vm.box = "sbeliakou/centos"
  ansblDay1h.vm.hostname = "ansblDay1-web"
  ansblDay1h.vm.network :private_network, ip: "192.168.56.81"
# ansblDay1h.vm.provision :shell, path: "apache.sh"
  ansblDay1h.vm.provider "virtualbox" do |vb|
    vb.name = "webserver"
    vb.memory = "2048"
    end
  end

config.vm.define "ansblDay1T" do |ansblDay1T|
  ansblDay1T.vm.box = "sbeliakou/centos"
  ansblDay1T.vm.hostname = "ansblDay1-app"
  ansblDay1T.vm.network :private_network, ip: "192.168.56.82"
# ansblDay1T.vm.provision :shell, path: "tomcat.sh"
  ansblDay1T.vm.provider "virtualbox" do |vb|
     vb.name = "appserver"
     vb.memory = "2048"
     end
  end
end