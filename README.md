Vagrant Multi-Machine (ubuntu 14.04) environment in headless mode

##### How to run
```
vagrant up

vagrant ssh
```

##### vagrant plugins installed
```
vagrant plugin install <plugin-name>
```

plugin-name:
```
vagrant-registration (1.3.1)
vagrant-service-manager (1.5.0)
vagrant-share (1.1.7, system)
vagrant-vbguest (0.13.0)
```

##### vagrant ssh-config
```
Host Vagrant-Ubuntu-14.04-1
  HostName 127.0.0.1
  User vagrant
  Port 2222
  UserKnownHostsFile /dev/null
  StrictHostKeyChecking no
  PasswordAuthentication no
  IdentityFile .vagrant/machines/Vagrant-Ubuntu-14.04-1/virtualbox/private_key
  IdentitiesOnly yes
  LogLevel FATAL
  ForwardAgent yes

Host Vagrant-Ubuntu-14.04-2
  HostName 127.0.0.1
  User vagrant
  Port 2200
  UserKnownHostsFile /dev/null
  StrictHostKeyChecking no
  PasswordAuthentication no
  IdentityFile .vagrant/machines/Vagrant-Ubuntu-14.04-2/virtualbox/private_key
  IdentitiesOnly yes
  LogLevel FATAL
  ForwardAgent yes

Host Vagrant-Ubuntu-14.04-3
  HostName 127.0.0.1
  User vagrant
  Port 2201
  UserKnownHostsFile /dev/null
  StrictHostKeyChecking no
  PasswordAuthentication no
  IdentityFile .vagrant/machines/Vagrant-Ubuntu-14.04-3/virtualbox/private_key
  IdentitiesOnly yes
  LogLevel FATAL
  ForwardAgent yes
```

##### For all available commands
```
vagrant --help
```

