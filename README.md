Ansible Role: Azure Devops (Pipeline) agent install
=========

Role install and configure Azure Devops Pipeline agent on Linux machines.

Requirements
------------

None.

Role Variables
--------------
Specify agent version:
```yaml
az_agent_version: 3.246.0
```
Specify user details. If not exists - role will create.
```yaml
az_agent_user: az-agent
az_agent_directory: /opt/az-agent/
```
Set this flag to allow reinstall agent if exists.
```yaml
az_agent_allow_reinstall_existing_agent: false
```


Dependencies
------------

None.

Example Playbook
----------------

No information needed.

License
-------

GPLv3

Author Information
------------------

Mateusz Pietrzak [mateoops](https://github.com/mateoops)
