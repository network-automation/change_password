# Change Password Example
This demonstration playbook shows how to easily automate changing a password for many switches simultaneously.  In Red Hat Ansible Tower the [survey tool](http://docs.ansible.com/ansible-tower/latest/html/userguide/job_templates.html#surveys) becomes really useful here.  In Red Hat Ansible Engine as shown here we can use the [prompt module](http://docs.ansible.com/ansible/latest/playbooks_prompts.html).

Run the playbook like this:
```bash
ansible-playbook password.yml
```

The playbook will ask the user two questions:
```bash
what user do you want to change?:
what is the password you want?:
```

It will then use the [nxos_config module](http://docs.ansible.com/ansible/latest/nxos_config_module.html) to change the password.

To view the playbook [click here](password.yml).

 ---
![Red Hat Ansible Automation](rh-ansible-automation.png)

Red Hat® Ansible® Automation includes three products:

- [Red Hat® Ansible® Engine](https://www.ansible.com/ansible-engine): a fully supported product built on the foundational capabilities of the Ansible project.

- [Red Hat® Ansible® Networking Add-On](https://www.ansible.com/ansible-engine): provides support for select networking modules from Arista (EOS), Cisco (IOS, IOS XR, NX-OS), Juniper (Junos OS), Open vSwitch, and VyOS.

- [Red Hat® Ansible® Tower](https://www.ansible.com/tower): makes it easy to scale automation, manage complex deployments and speed productivity. Extend the power of Ansible with workflows to streamline jobs and simple tools to share solutions with your team.

Want more info?
[Read this blog post for more info about Engine, the networking add-on and Tower](https://www.ansible.com/blog/red-hat-ansible-automation-engine-vs-tower)
