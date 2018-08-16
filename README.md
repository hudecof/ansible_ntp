# NTP

Ansible role to setup ntp service

## Requirements

- ansible: version 2 and higher

## Role Variables

in the variable `ntp_config_directives` defined in `vars/main.yml` are defined all supported `ntp.conf` variables with defautls. For each variable there is **name**, **type** and **default value**. 

To override the the default value set varibale `ntp_conf_<name>`, see some defaults in `defautls/main.yml`

If the type is

- **s** / **scalar**: use value enclosed in double quote, since values like **yes** and **no** have special meaning.
- **l** / **list**: use YAML list syntax, like `['val1', 'val2']`

There are some OS specific variables, which are defined in variables `__ntp_conf_<name>` in `vars/os-<distribution>` but still could be overwriten.

## Dependencies

None

## License

BSD

## Author Information

Peter Hudec