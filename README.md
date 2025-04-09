# compile-install-kernel

A simple script to automate my compilance of `sys-kernel/gentoo-sources`, PERSONAL USE ONLY!

The script was only tested on Gentoo Linux with the `sys-kernel/installkernel` configured to invoke `dracut` to generate a unified kernel image and install it in `systemd`'s kernel-install layout for `systemd-boot`. 

> This is my USE flags for `sys-kernel/installkernel`
> `sys-kernel/installkernel[dracut systemd systemd-boot uki]`

Please note that the configured `sys-kernel/installkernel` interprets the command `make install`.

## What does it do

The script will only do the compilance job!!!

That means you have to prepare the **kernel sources** and **configuration** in the desired working directory before you execute the script.

This script automates Linux kernel compilance and copies necessary files from current working directory to the symbolic link `/usr/src/linux` for out-of-tree module compilance and package manager to inspect.

> Compiling `sys-kernel/gentoo-sources` with Gentoo's default distribution kernel configuration from `sys-kernel/gentoo-kernel-bin` will need at least 23 GB of disk space.
>
> In my case, I usually do the compilance in `/tmp`, which means it takes up **23 GB of cached RAM**!
>
> So be CAUTIOUS if you want to use my script straightly.
