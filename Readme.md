# Ansible YUM

Simple role to patch a RHEL/Centos system and install default packages.

## Variables
```yaml
# default packages yum install comma separated
yum_default_packages                : ""

# Force update (use probably from CLI)
yum_upgrade_now_force               : False

# Reboot after system update
yum_reboot_if_needed                : True
yum_upgrade_now_pause_after_reboot  : 5

# SSH port to wait for instance to come back after a reboot
yum_upgrade_now_ssh_port            : "{{ ansible_port | default(22) }}"
```


# License
MIT

