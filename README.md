Travis-ci status: [![Build Status](https://secure.travis-ci.org/jackl0phty/ansible-role-nmap.png?branch=master)](http://travis-ci.org/jackl0phty/ansible-role-nmap)

Role Name
=========
# Nmap

Requirements
------------
Ansible core modules.

Description
-----------
[Ansible](http://www.ansible.com/home) role for installing the open source port scanner [Nmap](https://nmap.org/).

This Ansible role will install Nmap from source.

Role Variables
--------------
<pre><code>
Set type of install to do.
nmap_install_type: 'source'

Set version of Nmap is installed ( Used only for installing via source ).
vnmap_ersion: '6.47'

Nmap download URL ( Used only for installing via source ).
nmap_download_url: 'https://nmap.org/dist/nmap-{{ version }}.tar.bz2'
</pre></code>

Download and Install the Ansible Nmap role
------------------------------------------
<pre><code>
ansible-galaxy install jackl0phty.nmap
</pre></code>

Execute the Nmap role against your node
---------------------------------------
</pre></code>
ansible-playbook tasks/main.yml
</pre></code>

Dependencies
------------
None

Example Playbook
----------------
    - hosts: servers
      roles:
         - { role: jackl0phty.nmap, nmap_version: 6.4.7, nmap_install_type: source, nmap_download_url: https://nmap.org/dist/nmap-{{ version }}.tar.bz2 }

License
-------
Apache 2.0 'The License'.
