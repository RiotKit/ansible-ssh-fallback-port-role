SSH Fallback Port
=================

Allows to define a fallback SSH port, in case our playbook is for example reconfiguring the SSH server.

```bash
ansible-galaxy install blackandred.server_ssh_fallback_port
```

Example usage:
```yamlex
- hosts: all
  gather_facts: no
  remote_user: root
  roles:
      - name: blackandred.server_ssh_fallback_port
        vars:
            fallback_ssh_port: "6420"
```
