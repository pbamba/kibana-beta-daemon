Kibana Beta init script
==================

A simple init.d script that creates a [Kibana 4](http://www.elasticsearch.org/overview/kibana/installation/) (tested up to Beta 3) daemon.

Motivation
--------------

This script adresses the lack of system service to launch Kibana.
However, this issue will probably be addressed in future versions of Kibana (as mentionned in [here](https://github.com/elasticsearch/kibana/issues/1811)).


Getting started
---------------

Copy the "kibana" file to the /etc/init.d/ folder

Set the "DAEMON" variable with the path to the kibana bin file

Example: `DAEMON=/usr/share/kibana-4.0.0-beta3/bin/kibana`

Usage
---------------

### Start

`sudo service kibana start`

### Stop

`sudo service kibana stop`

### Restart

`sudo service kibana restart`

### Status

`sudo service kibana status`

Logging
---------------

Both standard and error outputs go to /var/log/kibana.log

License
-------

Copyright (C) 2014 Patrick Bamba

This is open source software, licensed under the MIT License. See the
file LICENSE for details.