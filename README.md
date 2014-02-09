Ansible Apache 2.4 Ubuntu Saucy Playbook
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

Example:

```
production                # inventory file for production servers
stage                     # inventory file for stage environment

group_vars/
   group1                 # here we assign variables to particular groups
   group2                 # ""
host_vars/
   hostname1              # if systems need specific variables, put them here
   hostname2              # ""

site.yml                  # master playbook
webservers.yml            # playbook for webserver tier
dbservers.yml             # playbook for dbserver tier

roles/
   apache2 # Here is where apache 2 playbook should be added along with other roles

    webtier/              # same kind of structure as "common" was above, done for the webtier role
    monitoring/           # ""
    fooapp/
```

Now that you have a nice structure add the role to the roles dir. Or you can install it via ansible galaxy. Either-ways just add the book and the role to your webtier or the the correct playbook.

After that, go to the default variables and edit the Vhosts with your preferences. You can also just override them via settings them in ```group_vars``` or ```host_vars```

That's it. Enjoy