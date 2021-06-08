## Create setup VM

- Create and configure Virtual machine `vagrant up`
- Configure the vm box ```Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"end```
- Shut down the running machine `vagrant halt`
- To suspend the running machine rather than shutting down fully `vagrant suspend`
- To access the running vagrant machine `vagrant ssh`
- To check the status of the running VM `vagrant status`
- To clean up all the resources that was created dusring vm creation process `vagrant destroy`
- To update the vm `sudo apt-get update -y`
- To exit the vm `exit`
