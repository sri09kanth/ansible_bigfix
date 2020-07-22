bigfix [![circleci](https://circleci.com/gh/GSA/ansible-bigfix.svg?style=svg)](https://circleci.com/gh/GSA/ansible-bigfix)
=========

The BigFix application provides software use analysis and configuration management capabilities by capturing CDM information from the clients installed on endpoints. This ansible role installs and configures the agent required to communicate with client machines.

Requirements
------------

Required Packages
- besagent.rpm - linux installer package
- bigfix.exe - windows installer package

Role Variables
--------------

- redhat_bigfix_agent_filename: #redhat installer msi
- windows_bigfix_agent_filename: #windows installer msi

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - ansible-bigfix
```

Public domain
-------------

This project is in the worldwide [public domain](LICENSE.md). As stated in [CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
