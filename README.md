# zbx-debian
Debian UserParameters
=====================

Userparameters specific for debian based hosts.

Introduction
------------

Debian Userparams provide a set of userparameters usefull to inspect and make a extended monitoring over a debian system.

With this solution, you can have more info about your systems inside our zabbix.

Requirements
------------

For now, there is no requirements.

Installation
------------

To install this solution you'll need to do the following steps:

1. Clone the repository into a folder (using git clone command);
2. Copy 'docker.conf' into your zabbix agent configuration directory (/etc/zabbix/zabbix.conf.d/ if using official packages from zabbix sia);
3. Restart Zabbix Agent.

How to use
----------

For now, the following user parameters are provided:

 *  so.packages.upgrade.list: Get the list of upgradable packages on the system (usefull to verify if some critical package can be updated, creating good triggers);
 *  so.packages.upgrade.count: Get the number of upgradable packages.

Other info
----------

If you need the same info for Redhat Based Systems, you can use https://github.com/gcavalcante8808/zbx-centos instead.
