sshove
======

sshove is a wrapper around ssh and other tools to make using ssh easier and managing personal configuration automatically without introducing any manual tasks into your workflow.

Installation
------------

Save a copy of [sshove](https://github.com/therevmj/sshove/blob/master/bin/sshove) in a directory (preferably in your path).

Configuration
-------------

There are three primary configuration files.  These all live in '~/.ssh/sshove/'.  None of these files are required, but you will not get the full benefit of sshove with some configuration.
* sshove.conf

  This configuration file controls the behavior of sshove.  Must be parsable by /bin/sh and is sourced directly into sshove.   Typically you should only use this file to set varaibles that are used interally in sshove, but any 'sh' compatible
code is acceptable.

* include

  This file should contain a list of files and diretories that should be rsynced to any machine that you connect to using sshove.

* exclude

  This file should contain a list of files and directories that should NOT be rsynced to any machine that you connect to using sshove.

Basice Usage
------------

sshove [ssh options]

