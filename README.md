VSTS-Agent
==========

[![Build Status](https://travis-ci.org/angrox/ansible-role-vsts-agent.svg?branch=master)](https://travis-ci.org/angrox/ansible-role-vsts-agent)



**_This is a rework of the vsts-agent role from https://github.com/sigio/ansible-role-vsts-agent. After my pull request was not accepted, commented or rejected for a long time I assume the role was abandoned._**





A role to install and configure the VSTS-agent (Microsoft Visual Studio Team Services Build and Release Agent) for RedHat Enterprise 7.2+ and Debian OS Family



Requirements
------------

python-pip to install a newer version of pexpect and libcurl4-gnutls-dev for Debian OS Family. Also rh-git29 is installed from software-collections, as VSTS requires a newer version of git.

Role Variables
--------------

At a minimum, override the variables vsts_accountname and vsts_poolname to install the regular queue agent.  
To install a deployment group agent override the variables vsts_accountname ,vsts_projectname and vsts_deploymentgroupname.

Other variables are documented in the defaults/main.yml file.

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: angrox.vsts-agent }

License
-------

MIT

Author Information
------------------

github: angrox
