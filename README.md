# Vagrant - Rocky Linux 9.1 Template

## About 
This template have the Rocky Linux base OS with a useful tools. 
- htop
- epel-release
- net-tools
- netcat
- yum utils
- docker repository (no docker engine, only the repo)
- gcc, make, perl, kernel-headers & devel, bzip2, zip, dkmsansiblev
- box guest
 
## Default Credentials
- Username: root
- Pass: passwd

## Usage / Running
For usage, you need to to genetate ssh keys and change the path on Vagrantfile
```sh 
$ ssh-keygen
```
and then run:
```sh
$ vagrant up
```
```sh
C:\Projects>cd vagrant-rocky9
C:\Projects\vagrant-rocky9>code Vagrantfile
C:\Projects\vagrant-rocky9>vagrant up
Bringing machine 'rocky' up with 'virtualbox' provider...
==> rocky: Box 'jarlley/rocky9' could not be found. Attempting to find and install...
    rocky: Box Provider: virtualbox
    rocky: Box Version: >= 0
==> rocky: Loading metadata for box 'jarlley/rocky9'
    rocky: URL: https://vagrantcloud.com/jarlley/rocky9
==> rocky: Adding box 'jarlley/rocky9' (v1.0) for provider: virtualbox
    rocky: Downloading: https://vagrantcloud.com/jarlley/boxes/rocky9/versions/1.0/providers/virtualbox.box
    rocky:
    rocky: Calculating and comparing box checksum...
==> rocky: Successfully added box 'jarlley/rocky9' (v1.0) for 'virtualbox'!
==> rocky: Importing base box 'jarlley/rocky9'...
==> rocky: Matching MAC address for NAT networking...
==> rocky: Checking if box 'jarlley/rocky9' version '1.0' is up to date...
==> rocky: Setting the name of the VM: vagrant-rocky9_rocky_1675434535607_4886
==> rocky: Fixed port collision for 22 => 2222. Now on port 2200.
==> rocky: Clearing any previously set network interfaces...
==> rocky: Preparing network interfaces based on configuration...
    rocky: Adapter 1: nat
    rocky: Adapter 2: bridged
==> rocky: Forwarding ports...
    rocky: 22 (guest) => 2200 (host) (adapter 1)
==> rocky: Running 'pre-boot' VM customizations...
==> rocky: Booting VM...
==> rocky: Waiting for machine to boot. This may take a few minutes...
    rocky: SSH address: 127.0.0.1:2200
    rocky: SSH username: root
    rocky: SSH auth method: password
    rocky:
    rocky: Inserting generated public key within guest...
    rocky: Removing insecure key from the guest if it's present...
    rocky: Key inserted! Disconnecting and reconnecting using new SSH key...
==> rocky: Machine booted and ready!
[rocky] GuestAdditions 7.0.4 running --- OK.
==> rocky: Checking for guest additions in VM...
==> rocky: Configuring and enabling network interfaces...
==> rocky: Mounting shared folders...
    rocky: /vagrant => C:/Projects/vagrant-rocky9
==> rocky: Running provisioner: shell...
    rocky: Running: inline script
    rocky: Last metadata expiration check: 3:28:01 ago on Fri Feb  3 11:01:53 2023.
    rocky: Dependencies resolved.
    rocky: Nothing to do.
    rocky: Complete!
```
