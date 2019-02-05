# Udemy Python Environment

So, I've subscribed to Udemy [Complete Python Bootcamp] and did not want to clutter my machine with software.

This repository contains all details to setup a virtual machine to install all software on.

## Download Ansible roles

```
ansible-galaxy install -r roles/requirements.yml
```

## Start the machine

```
vagrant up
```

## Configure the machine

```
./playbook
```

## Learn!

Either login to the VM:

```
vagrant ssh
```

Or use Jupyter Notebook by visiting the IP address of the virtual machine.

Hint 1: Find the IP of the vm using `vagrant ssh-config`.
Hint 2: Find the access token using `systemctl status jupyter-notebook` on the virtual machine.
