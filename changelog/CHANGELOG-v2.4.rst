=========================================
vbotka.freebsd_timezone 2.4 Release Notes
=========================================

.. contents:: Topics

2.4.0
=====

Release Summary
---------------
Unified namespace bsd_tz_*. Unified formatting of rc.conf options. Add
status reports bsd_tz_stat_zoneinfo and bsd_tz_stat_ntpdate. Variable
bsd_tz_ntpdate_enable is Boolean not a string. Simplified debug in
timezone blocks.

Major Changes
-------------
* Update to Ansible 2.14
* Add status reports bsd_tz_stat_zoneinfo and bsd_tz_stat_ntpdate.
* Simplified debug in timezone blocks.

Breaking Changes
----------------
* Unified namespace bsd_tz_*
* Unified formatting of rc.conf options
* Variable bsd_tz_ntpdate_enable is Boolean not a string.
