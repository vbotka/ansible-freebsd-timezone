freebsd-timezone
================

[![Build Status](https://travis-ci.org/vbotka/ansible-freebsd-timezone.svg?branch=master)](https://travis-ci.org/vbotka/ansible-freebsd-timezone)
[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)

[Ansible role.](https://galaxy.ansible.com/vbotka/freebsd-timezone/) Configures FreeBSD timezone.

Tested with FreeBSD 10.3 at [digitalocean.com](https://cloud.digitalocean.com)


Requirements
------------

No requiremenst.


Variables
---------

TBD (Check the defaults).


Workflow
--------

1) Change shell to /bin/sh.

```
ansible mailserver -e 'ansible_shell_type=csh ansible_shell_executable=/bin/csh' -a 'sudo pw usermod freebsd -s /bin/sh'
```

2) Install role.

```
ansible-galaxy install vbotka.ansible-freebsd-timezone
```

3) Fit variables.

```
~/.ansible/roles/vbotka.ansible-freebsd-timezone/vars/main.yml
```

4) Create playbook.

```
> cat ~/.ansible/playbooks/freebsd-timezone.yml
---
- hosts: mailserver
  become: yes
  become_method: sudo
  roles:
    - role: vbotka.ansible-freebsd-timezone
```

5) Configure the timezone.

```
ansible-playbook ~/.ansible/playbooks/freebsd-timezone.yml
```

License
-------

BSD


Author Information
------------------

[Vladimir Botka](https://botka.link)


References
----------

[How time is affected by the ntpd and /etc/localtime](http://serverfault.com/questions/303517/how-time-is-affected-by-the-ntpd-and-etc-localtime)
