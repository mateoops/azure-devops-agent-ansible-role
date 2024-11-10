Ansible Role: Azure Devops (Pipeline) agent install
=========

Role install and configure Azure Devops Pipeline agent on Linux machines.

Requirements
------------

None.

Role Variables with default values
--------------
Set organization url (for Azure Pipelines: https://dev.azure.com/{yourorganization})
```yaml
az_agent_server_url: null
```
Set user PAT (generation instructions: [LINK](https://learn.microsoft.com/en-us/azure/devops/pipelines/agents/personal-access-token-agent-registration?view=azure-devops#create-a-personal-access-token-for-agent-registration))
```yaml
az_agent_pat: null
```
Specify agent version:
```yaml
az_agent_version: 3.246.0
```
Provide name of **existing** agent pool
```yaml
az_agent_pool_name: Default
```
Specify user details. If not exists - role will create.
```yaml
az_agent_user: az-agent
az_agent_directory: /opt/az-agent/
```
Set this flag to allow reinstall agent if exists.
:warning: Before reinstalling make sure the agent has been removed from the pool
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
