# VirtualHere server install and uninstall script

VirtualHere server install script for `systemd` based systems (e.g Raspberry
Pi and most modern Linux Distributions).

## Installing default version

To install the default server version for your architecture, run the following
command and enter in your sudo password when prompted.

    curl https://raw.githubusercontent.com/virtualhere/script/main/install_server | sudo sh

## Installing optimized or custom version

To install an optimized or custom version, pass the file name as a script
argument. A list of optimized versions is available in the "CPU optimized
builds of VirtualHere USB Server for Maximum Performance on your hardware"
section of [Linux USB Server](https://www.virtualhere.com/usb_server_software)
page.

    curl https://raw.githubusercontent.com/virtualhere/script/main/install_server | sudo sh -s - vhusbdarmpi4

## Uninstalling server

To uninstall the server, run the following command. This script will remove
server binary and systemd service, but it will preserve the configuration file.

    curl https://raw.githubusercontent.com/virtualhere/script/main/uninstall_server | sudo sh
