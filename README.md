# collectiveaccess_ansible
Ansible playbook and roles to deploy Collective Access Providence and Pawtucket2

# overview
This playbook and its supporting roles will create a unified installation of Collective Access on top of Apache httpd, using mysql. By default, it will deploy with version 7.4.x of PHP, version 1.7.17 of Providence, and 1.7.15 of Pawtucket2.

# platform
As written, this playbook should work fine on Red Hat Enterprise Linux 8 and derivatives thereof (Alma/Rocky/etc.)

# requirements
Use the supplied `requirements.yml` to install the required roles.

# configuration
At a minimum, copy `group_vars/all.yml-example` to `group_vars/all.yml`, and set the marked variables (email, site name and passwords). You will also need to create an Ansible inventory with a host or group called 'ca' where you would like Collective Access to be installed.

# contact
Please let me (Alexander Jacocks) know, or better, open an issue and pull request, if you find any problems. Feel free to offer suggestions, as well.