# SAP Machine (OpenJDK distro)

[https://github.com/SAP/SapMachine](github.com/SAP/SapMachine) is one of OpenJDK distros, provided by SAP.

## 概要

This role installs SAP Machine to hosts.

## Supported versions

- Ubuntu 20.04 (bionic)
- ansible>=2.10,<2.11
- Jinja2>=2.11,<2.12

## How to use

### Role variables

See also [Installation - SAP/SapMachine Wiki](https://github.com/SAP/SapMachine/wiki/Installation).

```yaml
sap_machine_package: "sapmachine-11-jdk"
```

<br>

### Example playbook

```yaml
- hosts:
    - servers
  become: True
  roles:
    - { role: sap_machine, tags: ["sap_machine", "java"] }
```

## Licence
MIT

