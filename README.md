# Step by step tutorial
- Initialize a Vagrant Env in desired location ```vagrant init```
- Change Vagrantfile file to 
```
Vagrant.configure("2") do |config|
config.vm.box = "ubuntu/xenial64"
config.vm.box "private_network", ip:192.168.10.100"
end
```
- Create Virtual machine ```vagrant up```
- To check the status of the running VM ```vagrant status```
- To access the running vagrant machine ```vagrant ssh```
- To update the vm ```sudo apt-get update -y```
- To install nginx ```sudo apt-get install nginx -y```
- To test the private network setup got the browser and type in the ip: ```192.168.10.100```

# Other handy commands
- To exit the vm directory ```exit```
- To clean up all the resources that was created dusring vm creation process ```vagrant destroy```, you need to be outside vm terminal
