
check_fs_writeable
==================

This check plugin for Nagios / Icinga / Icinga2 checks for the writeability of
filesystems. As ext4 typically is mounted with **errors=remount-ro** which is in
itself a good idea, VM migration and storage timeouts may cause an accidential
remounting to read-only.

	$ ./check_fs_writeable --help
	check_fs_writeable [-pt] [long options...] <some-arg>
		-p STR... --path STR...  Path to check
		-t INT --timeout INT     Timeout

		--help                   print usage message and exit


Installation
------------

You need some perl packages for this script to work:

    apt-get install libgetopt-long-descriptive-perl \
    		libmonitoring-plugin-perl

