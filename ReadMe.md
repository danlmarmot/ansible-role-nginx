An Ansible role for installing nginx on Ubuntu 15.10.

### Default versions

Ubuntu 15.10
nginx 1.9.3

### Testing

A Vagrant/VirtualBox environment is provided in the /examples directory.  To get started:

1. Install Vagrant, Virtualbox, and Ansible
1. Change your directory into 'examples'
1. Run 'vagrant up' to bring up the VM.

### Additional notes

- For Vagrant installs, the install packages for nginx are downloaded once and cached locally.
- Each role in this Ansible playbook will check the version of each application before installing, and will not re-install if the installed version is the desired version.  This speeds up reprovisioning.
- To reprovision, use the 'vagrant provision' command.
