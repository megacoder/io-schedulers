io-schedulers
=============

What
----

A small zsh(1) script to display each block device name and its chosen I/O scheduler.

How
---

	$ io-scheduler
	/dev/sda	noop deadline [cfq]
	...
	/dev/sr0	noop deadline [cfq]

Why
---

Curious sysadmins want to know.

The strategy used to determine the order that disk blocks are written can have a significant impact on the overall system throughput.  The I/O scheduler can be changed at any time (by root) but get reset to a default every system boot.
