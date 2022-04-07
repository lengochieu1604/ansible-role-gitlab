# ANSIBLE ROLE GITLAB
-------------------------
## Installs Gitlab for Ubuntu linux servers.
## Requirements
-------------------------
    OS: Ubuntu (16.04/18.04/20.04)
    Storage: The Omnibus GitLab package requires about 2.5 GB of storage space for installation.
    CPU: 4 cores is the recommended minimum number of cores and supports up to 500 users, 8 cores supports up to 1000 users
    Memory: 
      4GB RAM is the required minimum memory size and supports up to 500 users (Our Memory Team is working to reduce the memory requirement).
      8GB RAM supports up to 1000 user

## Role Variables
--------------
    None.

## Dependencies
------------
    None.

## Example Playbook
----------------
  - name: Install Gitlab
    hosts: linux
    vars_files:
      - role-gitlab/vars/main.yml
    become: true 
    # gather_facts: false 
    roles:
      - role-gitlab
    
## License
-------
    LÊ NGỌC HIẾU

## Author Information
------------------

    This role was created in 2022 by Lê Ngọc Hiếu from Việt Nam, Devops Engineer

