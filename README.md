# freebsd_timezone

[![quality](https://img.shields.io/ansible/quality/27910)](https://galaxy.ansible.com/vbotka/freebsd_timezone)[![Build Status](https://travis-ci.org/vbotka/ansible-freebsd-timezone.svg?branch=master)](https://travis-ci.org/vbotka/ansible-freebsd-timezone)

[Ansible role.](https://galaxy.ansible.com/vbotka/freebsd_timezone/) FreeBSD. Configure timezone.

Feel free to [share your feedback and report issues](https://github.com/vbotka/ansible-freebsd-timezone/issues).

[Contributions are welcome](https://github.com/firstcontributions/first-contributions).


## Requirements

None.


## Variables

Review the defaults and examples in vars.


## Workflow

1) Change shell to /bin/sh

```
shell> ansible srv.example.com -e 'ansible_shell_type=csh ansible_shell_executable=/bin/csh' -a 'sudo pw usermod freebsd -s /bin/sh'
```

2) Install role

```
shell> ansible-galaxy install vbotka.freebsd_timezone
```

3) Fit variables

```
shell> editor vbotka.freebsd_timezone/vars/main.yml
```

4) Create playbook

```
shell> cat freebsd-timezone.yml

- hosts: srv.example.com
  roles:
    - vbotka.freebsd_timezone
```

5) Configure the timezone

```
shell> ansible-playbook freebsd-timezone.yml
```


## References

[How time is affected by the ntpd and /etc/localtime](http://serverfault.com/questions/303517/how-time-is-affected-by-the-ntpd-and-etc-localtime)


## License

[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)


## Author Information

[Vladimir Botka](https://botka.info)
