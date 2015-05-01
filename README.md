# ansible-role-nmap
[Ansible](http://www.ansible.com/home) role for installing the open source port scanner [Nmap](https://nmap.org/).

This Ansible role will install Nmap from source.

# Role Default Variables
<pre><code>
Set type of install to do.
install_type: 'source'

Set version of Nmap is installed ( Used only for installing via source ).
version: '6.47'

Nmap download URL ( Used only for installing via source ).
download_url: 'https://nmap.org/dist/nmap-{{ version }}.tar.bz2'
</pre></code>

# Download and Install the Ansible Nmap role.
<pre><code>
ansible-galaxy install jackl0phty.nmap
ansible-playbook jackl0phty.nmap/tasks/main.yml
</pre></code>

# Execute the Nmap role against your node.
</pre></code>
ansible-playbook jackl0phty.nmap/tasks/main.yml
</pre></code>