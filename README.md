Ansible role: vector
=========

This role installs vector on the server.


Role Variables
--------------

User variables are located in (defaults/main.yml[defaults/main.yml])

| Name | Default Value | Description |
|------|---------------|-------------|
| vector_version | 0.31.0 | Vector package version |
|------|---------------|-------------|
| vector_dir | /etc/vector | Path to directory with vector configuration |
|------|---------------|-------------|
| vector_data_dir | /var/lib/vector | Path to directory with vector data |
|------|---------------|-------------|
| vector_tmp_dir | /tmp/vector | Path to directory for temporary installation files |


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - vector

License
-------

This project is licensed under MIT License.

Author Information
------------------

Kirill B.
