# ansible-aws-timesync-ntp #

Ensure chrony ntp is installed.

## Requirements ##

None.

## Role Variables ##

### Default ###

    - name: chrony_ntp_server
      desc: ntp server to use by chrony
      value: "169.254.169.123"

### Vars ###

    - name: chrony_conf_file
      desc: default path to chrony configuration file
      value: "/etc/chrony/chrony.conf"

    - name: chrony_service_name
      desc: default service name
      value: "chrony"

## Dependencies ##

None.

## Example Playbook ##

    - hosts: all
      roles:
        - role: ansible-aws-timesync-ntp
