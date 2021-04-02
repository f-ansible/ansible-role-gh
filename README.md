# Ansible role: Github cli

[![CI](https://github.com/f-ansible/ar-role-gh/workflows/CI/badge.svg?event=push)](https://github.com/f-ansible/ar-role-gh/actions?query=workflow%3ACI)

Installs [ Github cli ](https://github.com/cli/cli),  GitHub’s official command line tool on any RHEL/CentOS or Debian/Ubuntu Linux system.

## Requirements

None

## Role Variables

Role variables are in [defaults/main.yml](defaults/main.yml):

```
gh_version: "1.8.0"
gh_system: "{{ansible_system | lower}}"
gh_arch: "amd64"

gh_install_from_source: false
gh_local_bin_path: "~/.local/bin"

```

## Dependencies

- [geerlingguy.git](https://galaxy.ansible.com/geerlingguy/git)

# Example Playbook

    - hosts: servers
      roles:
         - { role: fesaille.gh }

License
-------

BSD
