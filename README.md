## Question2Answer deployment

These playbooks deploy Question2Answer with Apache2 and MySQL for Ubuntu Xenial.

## Installation
- Ensure you have the correct credential and python2.7 on the server you want to install q2a.
- Edit the `hosts` inventory file to include the names or URLs of the servers you want to deploy.
- Configure the q2a credentials in `group_vars/all` file.

Run the playbook:

	ansible-playbook -i hosts site.yml -e 'ansible_python_interpreter=/usr/bin/python2.7'