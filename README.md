fuse-rofs
=========

ROFS is the Read-Only File System for FUSE. You can mount it over any filesystem that Linux can mount.

Copyright 2005,2006,2008 Matthew Keller. m@cognusion.com and others.

Mount any filesytem, or folder tree read-only, anywhere else.
No warranties. No guarantees. No lawyers.

I read (and borrowed) a lot of other FUSE code to write this. 
Similarities possibly exist- Wholesale reuse as well of other GPL code.
Special mention to RÃ©mi Flament and his loggedfs.

Consider this code GPLv2.

Compile: gcc -o rofs -Wall -ansi -W -std=c99 -g -ggdb -D_GNU_SOURCE -D_FILE_OFFSET_BITS=64 -lfuse main.c
Mount: rofs readwrite_filesystem mount_point

