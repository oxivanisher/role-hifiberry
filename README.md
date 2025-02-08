hifiberry
=========

Configure hifiberry addon for Raspberry Pi.

Role Variables
--------------

| Name             | Comment                           | Default value                   |
|------------------|-----------------------------------|---------------------------------|
| hifiberry_dtoverlay    | The dtoverly to be used | `hifiberry-dac` |
| hifiberry_rpi_boot_dev | The boot device where the `config.txt` is located. Will be overwritten if `raspberry_pi_boot_dev` is set! | `/de`/mmcblk0p1` |


Example Playbook
----------------
```yaml
- name: Configure hifiberry
  hosts: all
  collections:
    - oxivanisher.raspberry_pi
  roles:
    - role: oxivanisher.raspberry_pi.hifiberry
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.raspberry_pi](https://galaxy.ansible.com/ui/repo/published/oxivanisher/raspberry_pi/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-raspberry_pi).
