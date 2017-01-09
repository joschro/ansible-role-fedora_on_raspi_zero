fedora_on_raspi_zero
====================

A brief description of the role goes here.

Requirements
------------

1. Get Pignus (pignus-minimal-23a.xz) from https://pignus.computer/pub/linux/pignus/releases/23/images/
2. Write image on SD card: xz -cd "pignus-minimal-23a.xz" | dd of=/dev/sdb bs=4M
3. Boot Raspi with SD card inserted and USB-2-LAN adapter
4. Login with root and no/empty password
5. Set new password: passwd
6. Note IP address of eth0: <ip add sh>
7. Run either locally or remote via SSH: dnf install ansible git
8. Run: git clone https://github.com/joschro/ansible-role-fedora_on_raspi_zero

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
