# lv_remover

This role is designed to remove LVMs found by there mount points. It takes array of mount points as an argument and then findes related LVMs in fstab.

##### example

```yml
- hosts: all
  become: yes
  become_method: sudo
  roles:
      - { role: lv_remover, lv_remover_mounts: ['/deleteme','/mount/rdisk2'] }
```
