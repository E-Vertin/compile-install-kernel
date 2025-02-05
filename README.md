# compile-install-kernel
A simple script to automate my compilance of `sys-kernel/gentoo-sources`, PERSONAL USE ONLY!

## What does it do

This script automates Linux kernel compilance and copies necessary files from /tmp/linux to /usr/src/linux for out-of-tree module compilance.

> Compiling `sys-kernel/gentoo-sources` with Gentoo's distribution kernel configuration will need at least 23 GB of disk space.
>
> In my case, I usually do the compilance in `/tmp`, which means it takes up **23 GB of RAM**!
>
> So be CAUTIOUS if you want to use my script straightly.

The script will only do the compilance job!!!

That means you have to prepare the **kernel source** and **configuration** in a directory before you execute the script.