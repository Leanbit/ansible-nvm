leanbit.nvm
=========

Install and Updata NVM, install multiple node version and multiple packages.


Role Variables
--------------

    nvm_version: "v0.31.3"
    nvm_default_node_version: "6.3.0"
    nvm_node_versions: 
      - "{{nvm_default_node_version}}"
    nvm_user: ubuntu
    nvm_npm_pkgs: 
      - pkg: bower
        version: "1.7.9"


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - role: leanbit.nvm
      nvm_user: ubuntu
      nvm_version: "v0.31.3"
      nvm_node_versions: 
        - 6.3.0 
        - 5.12.0
      nvm_npm_pkgs:
        - pkg: bower
          version: "*"

if you need to install on multiple linux users duplicate the role in your playbook.

License
-------

MIT

Author Information
------------------

Leanbit srl