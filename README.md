[![CI](https://github.com/de-it-krachten/ansible-role-awx_casc/workflows/CI/badge.svg?event=push)](https://github.com/de-it-krachten/ansible-role-awx_casc/actions?query=workflow%3ACI)


# ansible-role-awx_casc

Import AWX configuration using Configuration-as-Code 



## Dependencies

#### Roles
None

#### Collections
- awx.awx

## Platforms

Supported platforms

- Red Hat Enterprise Linux 8<sup>1</sup>
- Red Hat Enterprise Linux 9<sup>1</sup>
- RockyLinux 8<sup>1</sup>
- RockyLinux 9<sup>1</sup>
- OracleLinux 8
- OracleLinux 9<sup>1</sup>
- AlmaLinux 8<sup>1</sup>
- AlmaLinux 9<sup>1</sup>
- Debian 10 (Buster)<sup>1</sup>
- Debian 11 (Bullseye)<sup>1</sup>
- Debian 12 (Bookworm)<sup>1</sup>
- Ubuntu 20.04 LTS<sup>1</sup>
- Ubuntu 22.04 LTS<sup>1</sup>
- Ubuntu 24.04 LTS<sup>1</sup>
- Fedora 41<sup>1</sup>

Note:
<sup>1</sup> : no automated testing is performed on these platforms

## Role Variables
### defaults/main.yml
<pre><code>
# Use non default virtual env
# awx_python_interpreter: /virtenv/awx/bin/python3

# For inventory/host/group, you can replace variable values during creation
# In order not to replace intended dynamic variables, use the following markers
# awx_variable_jinja_block_start: "<%"
# awx_variable_jinja_block_end: "%>"
# awx_variable_jinja_variable_start: "<="
# awx_variable_jinja_variable_end: "=>"

# Full path to the awxkit / awx command
awx_command: awx

# Host to execute code from
awx_execution_host: localhost

# Should creation of AWX hosts be created
awx_create_hosts: true

# Check if hosts exist in DNS
awx_host_dns_check: false

# List of hosts that no longer exists (dynamically created)
awx_hosts_non_existing: []

# AWX url
awx_url: https://127.0.0.1

# AWX username to use
awx_username: admin

# AWX password to use
awx_password: admin

# Should SSL/TLS verification be done
awx_verify_ssl: false

# Location where to get configuration files from
# awx_config_path: /tmp/awx

# Skip creating hosts and assigning hosts to groups
awx_casc_skip_hosts: false

# Forcingly recreate workflow templates
awx_workflow_job_template_recreate: false

# Format for variables & input files
awx_vars_format: json
awx_inputs_format: json

# List of resources to export
awx_casc_resources:
  - settings
  - organizations
  - credential_types
  - credentials
  - execution_environments
  - inventory
  - inventory_sources
  - { name: projects, ignore_errors: true }
  - { name: job_templates, ignore_errors: true }
  - notification_templates
  - organizations
  - teams
  - users
  - workflow_job_templates
  # - roles  ## not yet
  - schedules
  # - applications  ## not yet
  # - system_job_templates  ## not yet
  - hosts
  - groups
</pre></code>




## Example Playbook
### molecule/default/converge.yml
<pre><code>
- name: sample playbook for role 'awx_casc' pre playbook
  ansible.builtin.import_playbook: converge-pre.yml
  when: molecule_converge_pre is undefined or molecule_converge_pre | bool
- name: sample playbook for role 'awx_casc'
  hosts: all
  become: 'no'
  vars:
    awx_command: /usr/local/bin/awx
    awx_config_path: /tmp/awx-config
  tasks:
    - name: Include role 'awx_casc'
      ansible.builtin.include_role:
        name: awx_casc
</pre></code>
