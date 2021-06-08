## Create setup VM

- Create and configure Virtual machine `vagrant up`
- Configure the vm box 
```
Vagrant.configure("2") do |config|
config.vm.box = "ubuntu/xenial64"end
```
- Shut down the running machine `vagrant halt`
- To suspend the running machine rather than shutting down fully `vagrant suspend`
- To access the running vagrant machine `vagrant ssh`
- To check the status of the running VM `vagrant status`
- To update the vm `sudo apt-get update -y`
- To exit the vm `exit`

#### Setup a private network in VM box
- Congfigure the Vagrantfile
```
Vagrant.configure("2") do |config|
config.vm.box = "ubuntu/xenial64"
config.vm.box "private_network", ip:192.168.10.100"
end
```
- To clean up all the resources that was created dusring vm creation process `vagrant destroy`
- Run the vagrant again `vagrant up`
- Access the running vm `vagrant ssh`
- To install a program `sudo apt-get install file_name`
- To test the private network setup got the browser and type in the ip: `192.168.10.100`
