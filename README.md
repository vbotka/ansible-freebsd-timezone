freebsd_timezone
================

[![Build Status](https://travis-ci.org/vbotka/ansible-freebsd-timezone.svg?branch=master)](https://travis-ci.org/vbotka/ansible-freebsd-timezone)
[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)

[Ansible role.](https://galaxy.ansible.com/vbotka/freebsd_timezone/) FreeBSD. Configure timezone.


Requirements
------------

No requiremenst.


Variables
---------

TBD. Review the defaults and examples in vars.


Workflow
--------

1) Change shell to /bin/sh.

```
# ansible srv.example.com -e 'ansible_shell_type=csh ansible_shell_executable=/bin/csh' -a 'sudo pw usermod freebsd -s /bin/sh'
```

2) Install role.

```
# ansible-galaxy install vbotka.freebsd_timezone
```

3) Fit variables.

```
# editor vbotka.freebsd_timezone/vars/main.yml
```

4) Create playbook.

```
# cat freebsd-timezone.yml

- hosts: srv.example.com
  roles:
    - vbotka.freebsd_timezone
```

5) Configure the timezone.

```
ansible-playbook freebsd-timezone.yml
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
