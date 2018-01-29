Role Name
=========

Ansible role for installing and configuring EPEL repository.

Role Variables
--------------

```bash
epel_repo_url: "https://ftp.heanet.ie/mirrors/fedora/epel/{{ ansible_distribution_major_version }}/{{ ansible_architecture }}/"
epel_repo_gpg_key_url: "https://ftp.heanet.ie/mirrors/fedora/epel/RPM-GPG-KEY-EPEL-{{ ansible_distribution_major_version }}"
epel_repofile_path: "/etc/yum.repos.d/epel.repo"
epel_repo_name: epel
```

Example Playbook
----------------

An example of how to use the role:

    - hosts: all
      roles:
         - { role: epel-repo }


Author Information
------------------

[Jakub Jarosz](https://twitter.com/qba73)
