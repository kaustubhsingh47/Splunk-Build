# Splunk-Build


To modify the above script to be used with Ansible, we need to make several changes to ensure that it conforms to Ansible's best practices and requirements. Here are some recommended modifications:

Change the script extension to .sh.j2 to indicate that it's a Jinja2 template.
Remove the shebang line since Ansible runs the script with /bin/sh by default.
Replace all echo commands with the debug Ansible module.
Use Ansible variables instead of hardcoding values.
Replace all commands that modify the file system with corresponding Ansible modules.
Convert the script into an Ansible task.


