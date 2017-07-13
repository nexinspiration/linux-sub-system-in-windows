# Linux subsystem (Windows)

This repo's main objective is to capture and help setting up the Linux sub system and also other tips and tricks.

### Table of Contents

- [Setting up Linux Subsystem](#setting-up-linux-subsystem)
- [Installing Node](#installing-node)

## Setting up Linux Subsystem

### Prerequistes:
- 64 bit Version of Windows 10 Anniversary Update or later (build 1607+). You can check them in `Settings > System > About`

### Steps to enable
- Go to `Control panel > Turn on or off windows features`, a popup will show up; Enable the Linux subsystem available in the pop up.

- Open `Settings > Update and Security > For developers` and select developer mode

- Open Command Prompt and type `bash`. You will be prompted to install ubuntu on windows, Type 'y' to accept and the ubuntu file system will be installed

- After its installed, you can open ubuntu app from the start menu and enjoy using the sub system

## Installing Node
Note: `apt-get install nodejs` and `apt-get install npm` won't work properly and will install old updates of Node.js and npm.

Its not the problem with the subsystem, rather its the Ubuntu way of installing it.

Below are the steps to install Node.js & npm:

1) Command 1: `curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
sudo apt-get install -y nodejs`

The above command installs Node.js LTS 6+ and related npm package

#### Reference
[Node.js - How to Install in Ubuntu](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions)
