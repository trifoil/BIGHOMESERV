# BIGHOMESERV 🖥

TrueNAS scale tutorial for beginners.

Homeserv's big brother. Aimed at helping you to set up your infrastructure very easily.

Most of this tutorial comes from the official website : https://www.truenas.com/docs/scale/22.12/scaletutorials/toptoolbar/

For information, I use Fedora Linux 38 (Workstation Edition).

## Table of Contents

1. [Considerations](#considerations)
1. [Installation of TrueNAS Scale](#installation)
2. [Disk Management and RAID Configuration](#disk-management)
   1. [Disk Management](#disk-management)
   2. [RAID Configuration](#raid-configuration)
3. [Setting up a VPN with a Domain Name](#vpn-setup)
   1. [Domain Name Registration (e.g., using Infomaniak)](#domain-registration)
   2. [VPN Configuration](#vpn-configuration)
4. [DNS Configuration](#dns-configuration)
5. [User Management](#user-management)
6. [Installation and Setup of GitLab](#gitlab-setup)
7. [Conclusion](#conclusion)
8. [Sources]
9. []


By the time I got my first server up and running, I started computing school, and the school firewall blocks wireguard (here, wg-easy).

The method used by Nerd on the Street is using tls tunnelling to hide the vpn.

Here are the steps I had to do to set it up :

1) Install Debian 

Install Debian with docker on your Truenas machine. It's quite simple because the name of the image you pull is debian.

Then connect through ssh to your container.

2) Wireguard install

First, install wireguard

```
apt install wireguard
```
Then we can look at the Kernel version, but the one we pulled is supposedly generig and hence you don't need another one.

```
uname -r
```
3) Enable IPv4 forwarding

```

```

Sources :

https://nerdonthestreet.com/wiki?find=Set+Up+a+WireGuard+VPN+Server+with+WebSocket+Tunneling