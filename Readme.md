# Ansible YUM

Simple role to patch a Redhat/Centos system and install default packages.

## Variables
```yaml
# default packages tp install comma seperated
yum_default_packages                : ""

# Force update (use probably from CLI)
upgrade_now_force                   : False

# Reboot after system update
reboot_if_needed                    : True
upgrade_now_pause_after_reboot      : 5

# SSH port to wait for instance to come back after a reboot
upgrade_now_ssh_port                : "{{ ansible_port | default(22) }}"
```


# License
MIT
