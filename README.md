# LibreNMS Ansible Role

Import in playbook:
```yaml
- hosts: all
  roles:
      - { role: rhaamo.librenms_agent, become: true }
```

Default config:
```yaml
# Repository with LibreNMS Agent sources
librenms_agent_repository: 'https://github.com/librenms/librenms-agent.git'

# Which version to install, defaults to master
librenms_agent_version: 'master'

# check_mk scripts to deploy
# choice of available scripts: https://github.com/librenms/librenms-agent/tree/master/agent-local
librenms_agent_check_mk_scripts: []
```