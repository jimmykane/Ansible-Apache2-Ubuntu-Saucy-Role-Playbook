Ansible Apache 2.4 Ubuntu Saucy Role
========================================

This role will install Apache 2.4 and enable,disable, delete Vhosts on an Ubuntu Saucy64 installation.
------------------------------------------------------------------------------------------------------

You can get the code or install it with ansible galaxy

Get the code:
-------------

- github: [Ansible-Apache2-Ubuntu-Saucy-Role-Playbook](https://github.com/jimmykane/Ansible-Apache2-Ubuntu-Saucy-Role-Playbook)

- Ansible Galaxy: [Ansible-Apache2-Ubuntu-Saucy-Role](https://galaxy.ansible.com/list#/roles/355)

Install Only
----------
```$ ansible-galaxy install jimmykane.Ansible-Apache2-Ubuntu-Saucy-Role```

Some tips and how to use
------------------------

First build a structure of a project as described in [Ansible Best Practices](http://docs.ansible.com/playbooks_best_practices.html)

After that add the role to the roles dir. Or you can install it via ansible galaxy.

Look at the default variables and edit the Vhosts with your preferences.
You might also want to override them via setting them in ```group_vars``` or ```host_vars```


Don't forget to add include it as a role at your playbooks