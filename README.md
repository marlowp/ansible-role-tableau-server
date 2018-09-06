# Ansible Role: Tableau Server

Utilises the [Automated Installer](https://github.com/tableau/server-install-script-samples/tree/master/linux) to install Tableau Server on Debian/Ubuntu servers.

## Usage

Ideal for using with [Virtual Box](https://www.virtualbox.org/) and [Vagrant](https://www.vagrantup.com/) to spin up a local Tableau Server instance for development/prototyping. Configuration options can be found in `defaults/main.yml`. It is recommended that you update the password and registration details before use.

## Requirements

The guest machine must meet the minimum specifications for Tableau Server, which is currently:

* 8GB RAM
* 2 Cores

The role has only been tested on the following software:

* Ubuntu - 16.04
* Virtualbox - 5.2.16 r123759 (Qt5.6.2)
* Vagrant - 2.0.1
* Ansible - 2.6.2

## Example Playbook

    - hosts: servers
      roles:
        - tableau-server

## Additional Enhancements

* Add support for Redhat/CentOS servers.
* Make available in [Ansible Galaxy](https://galaxy.ansible.com/home)
* Add optional plays to install database drivers (such as SQL Server)
* General tidy-up (author is not an experienced Ansible user :)

## Licence

MIT
