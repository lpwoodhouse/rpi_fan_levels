# Ansible Role: rpi_fan_adjust

### Part of my Raspberry Pi cluster project

Sets the 4 levels of cpu temperature at which an increase in fan speed occurs.

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see ```defaults/main.yml```)
```shell
cpu_temp0: 75
cpu_temp1: 80
cpu_temp2: 85
cpu_temp3: 90
reboot_var: true
```
## Dependencies

None

## Example Playbook
```yaml
    - hosts: all
      vars:
        cpu_temp0: 60
        cpu_temp1: 65
        cpu_temp2: 70
        cpu_temp3: 75
        reboot_var: false
      roles:
        - rpi_fan_adjust
```

## License

GNU General Public Licence v3.0

## Author Information

This role was created in 2022 by [Lee Woodhouse](https://www.leewoodhouse.com/)
