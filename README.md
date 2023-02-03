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

## Usage
For usage, you need to to genetate ssh keys and change the path on Vagrantfile
```sh 
$ ssh-keygen
```
and then run:
```sh
$ vagrant up
```
