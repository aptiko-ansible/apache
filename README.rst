==============
Ansible-apache
==============

Overview
========

This is an Ansible role for installing apache on Debian. It also
optionally installs awstats.

It performs some essential configuration such as enabling several
apache modules, marking 301 redirections as non-cacheable, and changing
the default log format. Other than that, it doesn't do much and should
be combined with ``apache-vhost``.

Options
=======

- ``use_ferm``: If ``true``, it drops a configuration snippet in
  ``/etc/ferm/ansible-late`` in order to allow connections to ports 80
  and 443.  In this case you must also use ansible_ferm_. The default is
  ``true`` for backwards compatibility reasons.
- ``use_awstats``: If ``true``, it installs and configures awstats. The
  default is ``true`` for backwards compatibility reasons.

.. _ansible_ferm: https://github.com/aptiko-ansible/ferm

Meta
====

Written by Antonis Christofides

| Copyright (C) 2021 GRNET
| Copyright (C) 2011-2015 Antonis Christofides
| Copyright (C) 2014-2021 TEI of Epirus
| Copyright (C) 2015-2021 National Technical University of Athens

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see http://www.gnu.org/licenses/.
