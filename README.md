Checklist to create virtual machine
===========

Creating on VirtualBox
-----------

> To create virtual box machine, is needed to uncheck sound,
> video acceleration, and set a second Netword Card, using 
> host-only attachment. Installing follow these steps:

1.  Install OS normally;
2.  Set OpenSSH to install;
3.  Restarting new OS;
4.  Install SO updates;
5.  Install VBoxLinuxAdditions;
6.  Install build-essential git-core zsh;
7.  Edit sudo permissions to NOPASSWD:;
8.  Create ssh-key and export to github;
9.  Uploading host ssh key to guest authorized_keys;
10. Set zsh to default shell;

Creating on Vagrant
--------------

> To export to vagrant, will need follow some default behaviours
> like ssh port forward and others.

1. Export to vagrant
2. Add box to ~/.vagrant directory
3. Config Vagrantfile with forward_ports and others
4. Up them all \m/
