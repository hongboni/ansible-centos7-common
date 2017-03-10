## Ansible Role: Common
Common setup tasks for all RedHat/CentOS 7 servers

## Tasks
* Set SELinux to Enforcing Mode (immediate reboot to activate)
* Add a swap partition
* Harden sshd configuration
  * Disable root login
  * Disable password authentication
  * Add Sudo users with ssh keys login
  * Add non-default port for sshd (also set SELinux & firewalld config)
  * Limite port 22 only for Ansible controler host and Privarte IPs
* Update all existing packages
* Install user-defined base packages (ex: nano screen)
* Enable automatic yum updates of security patches (via yum-cron)
* Add global shell enhancements (custom aliases, vim configs)
* Set default timezone
* Set default hostname if defined

## License
BSD
