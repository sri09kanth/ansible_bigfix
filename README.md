grace-ansible-bigfix
=========

The BigFix application provides software use analysis and configuration management capabilities by capturing CDM information from the clients installed on endpoints. This ansible role installs and configures the agent required to communicate with client machines.

Requirements
------------

besagent.rpm - Linux rpm installer
bigfix.msi - Windows msi installer

Role Variables
--------------

#default agent path directory
win_agent_path: "C:\\Temp\\Agents"
lin_agent_path: "/opt/GSA/install_files"

#default agent log path directory
win_agent_logs: "C:\\Temp\\Agents\\Logs"

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - grace-ansible-bigfix

License
-------

MIT

Author Information
------------------

Lance White - GSA/GEO
