# 02_Intro_to_linux

A Crash Course in Linux

Pre-reqs: 
Google Account

or 

Admin access to your workstation


## Setup

If you already have access to a linux environment skip this part and proceed to part 2.

There are multiple ways to get access to a linux environment. 2 will be provided here, but feel free to use a different method if you prefer. 

[Cloud Method](cloudmethod.md) (recomended)

[Virtulbox Method](virtualbox_method.md)


## Part 1 Exploring Linux

1. Open the terminal on your linux workstation.

2. Enter the command to view your current location on the file system.

3. List all the contents of the folder you are currently in.

4. Navigate to the /usr/bin directory. What is normally contained in this folder?

5. Navigate back to your home directory and create a file called system_notes.txt

6. Add your systems hostname to the system_notes.txt file like this: hostename = [your_hostname_here]

7. Add your systems total ram to the system_notes.txt file like this: total_ram = [your_systems_total_ram_here]

8. Add your systems free diskspace to the system_notes.txt file like this: free_diskspace = [your_systems_free_diskpace_here]

9. Copy the system_notes.txt file to your Documents folder.

10. View the contents of your copy of the system_notes.txt file without opening the file.

## Part 2 Securing Linux

1. Install system updates and remove unused packages. This prevents bad actors from using known vulnerabilites on your system

```bash
sudo apt update

sudo apt dist-upgrade

sudo apt-get autoremove

sudo apt-get autoclean
```

2. Turn on the automatic updates. Keep your system patched and up to date. 

```bash
sudo apt-get install unattended-upgrades

sudo dpkg-reconfigure -plow unattended-upgrades
```

3. Enable firewall. 

```bash
sudo ufw enable
```

4. Lock down firefox
* Preferences > General > Network Settings > Enable DNS over HTTPS. Select custom and enter https://dns.quad9.net/dns-query

* Preferences > Privacy and Security. Disable autofill of Logins and Passwords

* Configure firefox to never remember history

* Configure to never Collect data

* Install the Privacy Badger firefox extension

* Install the HTTPS Everywhere extension

## Part 3 Configuring Linux

1. Install the [Docker](https://docs.docker.com/engine/install/ubuntu/)

2. Install [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

3. Install [Visual Studio Code](https://code.visualstudio.com/docs/setup/linux)

4. Install the [WhiteSource Advise Plugin](https://marketplace.visualstudio.com/items?itemName=whitesource.whitesource-advise

5. Install the [Security Scan Plugin](https://marketplace.visualstudio.com/items?itemName=shiftleftsecurity.shiftleft-scan)

6. Install the [Dependency Analytics Plugin](https://marketplace.visualstudio.com/items?itemName=redhat.fabric8-analytics)

7. [Setup GitHub and SSH](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh)


