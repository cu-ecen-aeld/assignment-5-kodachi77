# Overview

This repository contains assignment starter code for buildroot based assignments for the course Advanced Embedded Software Design, ECEN 5713

It also contains instructions related to modifying your buildroot project to use with supported hardware platforms.  See [this wiki page](https://github.com/cu-ecen-5013/buildroot-assignments-base/wiki/Supported-Hardware) for details.

## Install

First install mandatory software:

    sudo apt-get install build-essential ncurses-base ncurses-bin libncurses5-dev dialog git wget cpio unzip rsync bc screen

## Configure

Run:

    make menuconfig
    make linux-menuconfig

to configure your buildroot and linux installation. You can also run something like:

     make -C buildroot linux-update-defconfig BR2_LINUX_KERNEL_CUSTOM_CONFIG_FILE=../base_external/configs/aesd_linux.config

to save your custom config outside build tree.

