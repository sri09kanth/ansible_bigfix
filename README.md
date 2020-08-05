bigfix [![circleci](https://circleci.com/gh/GSA/ansible-bigfix.svg?style=svg)](https://circleci.com/gh/GSA/ansible-bigfix)
=========

This ansible role installs and configures the bigfix agent required to communicate with client machines.

Requirements
------------

Required Packages (this role requires access to the following packages/installers via an external repository)
- besagent.rpm - linux installer package
- bigfix.exe - windows installer package
- masthead.afxm - bigfix masthead file

Role Variables
--------------

### Windows

| Variable | Default | Purpose |
| ------ | ------ | ------ |
| windows_agent_path | "C:\Program Files (x86)\BigFix Enterprise\BES Client" | default windows install directory |
| windows_agent_log | "C:\Temp\Logs" | default agent windows log directory |
| windows_bigfix_agent_url | "" | windows installer msi |
| windows_bigfix_product_id | "" | windows product_id |

### Redhat

| Variable | Default | Purpose |
| ------ | ------ | ------ |
| redhat_agent_path | "/opt/BESClient" | default redhat install directory |
| redhat_bigfix_agent_url | "" | redhat installer rpm |
| windows_bigfix_product_id | "" | win_package using a url requires a product_id |

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - bigfix
```

Public domain
-------------

This project is in the worldwide [public domain](LICENSE.md). As stated in [CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
