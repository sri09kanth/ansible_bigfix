ansible-bigfix
=========

The BigFix application provides software use analysis and configuration management capabilities by capturing CDM information from the clients installed on endpoints. This ansible role installs and configures the agent required to communicate with client machines.

Requirements
------------

```bash
redhat_bigfix_agent_filename: #redhat installer msi
windows_bigfix_agent_filename: #windows installer msi
```

Role Variables
--------------
```bash
None
```

Dependencies
------------
Acquire Installers
```bash
besagent.rpm - linux installer package
bigfix.exe - windows installer package
```

Example Playbook
----------------

```bash
    - hosts: servers
      roles:
         - ansible-bigfix
```

License
-------

MIT

Author Information
------------------

Lance White - GSA/GEO
