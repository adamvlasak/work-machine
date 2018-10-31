# working machine

## Overview

This project provisions your CentOS based OS for better user experience.

## Provisioning via ansible

This step assumes you have root access, you can SSH to your machine, you know its IP address and it runs CentOS. Please copy your id_rsa, id_rsa.pub and create authorized_keys in your /root/.ssh directory.

```
$ yum install git vim ansible
$ mkdir src && cd src
$ git clone git@github.com:adamvlasak/work-machine.git
$ cd work-machine/
$ make prepare
```

You must edit the file vars.yml according to your needs! Then run playbook:

```
$ make provision
```

Done!
