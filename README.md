This repository includes everything necessary to build a local environment that serves a simple "Hello World" flat HTML page.

This environment was built on Mac OS X Sierra using the following tools:
 - VirtaulBox
 - Vagrant
 - Ansible
 - TravisCI
 
 Prerequisites: required software
  - Xcode (latest, gcc and other tools needed to install ansible)
  - VirtualBox - https://www.virtualbox.org/wiki/Downloads
  - Ansible - installed using pip install
  - Python (Python 2.7.10, likely already installed)
  
  Ansible roles:
   - CIS Hardening guide - https://github.com/MindPointGroup/RHEL7-CIS.git
   - Firewalld - https://galaxy.ansible.com/geerlingguy/firewall/
   - Apache - https://galaxy.ansible.com/geerlingguy/apache/
   
You can clone this repository to a computer running Mac OS X Sierra and start the VirtualBox VM using Vagrant with the flag to provision the VM.  Run the follwing command in the directory where you cloned this repository:

    vagrant up --provision
   
   
   
