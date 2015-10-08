==============
Ansible-apache
==============

Overview
========

This is an Ansible role for installing apache on Debian. It also
installs awstats.

It performs some essential configuration such as enabling several
apache modules, marking 301 redirections as non-cacheable, and changing
the default log format. Other than that, it doesn't do much and should
be combined with ``apache-vhost``.

Meta
====

Written by Antonis Christofides

| Copyright (C) 2011-2015 Antonis Christofides
| Copyright (C) 2014 TEI of Epirus
| Copyright (C) 2015 National Technical University of Athens

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
