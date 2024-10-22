# MAC Address Changer

This is a simple Python script that allows you to change the MAC address of a network interface on Linux systems. It can be useful for security purposes, privacy, or when troubleshooting network issues.

## Features
- Display the current MAC address of a specified network interface.
- Change the MAC address to a user-specified value.
- Validate if the MAC address has been successfully changed.

## Prerequisites
- Python 3.x
- Linux-based operating system
- Root privileges (required to change MAC addresses)

## Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/mac_changer.git
cd mac_changer
```

## Usage

Run the script with superuser privileges to change the MAC address of your network interface.

```bash
sudo python3 mac_changer.py -i <interface> -m <new_mac_address>
```

### Arguments:
- `-i` or `--interface`: The network interface you want to modify (e.g., `eth0`, `wlan0`).
- `-m` or `--mac`: The new MAC address you want to assign (e.g., `00:11:22:33:44:55`).

### Example:

```bash
sudo python3 mac_changer.py -i wlan0 -m 00:11:22:33:44:55
```

### Output:
- The script will display the current MAC address, attempt to change it, and verify if the change was successful.

## Notes:
- The script currently supports only Linux systems where the `ifconfig` or `ip` command is available.
- Ensure that the MAC address format is valid (e.g., `XX:XX:XX:XX:XX:XX`).

## Troubleshooting:
- If you encounter any errors related to permissions, make sure you're running the script with `sudo` or as root.
- On newer Linux distributions, consider using the `ip` command instead of `ifconfig`. The script can be modified for this easily by replacing the `ifconfig` commands.

## License
This project is licensed under the MIT License.

## About

This script is part of the course [Learn Python & Ethical Hacking from Scratch](https://www.udemy.com/course/learn-python-and-ethical-hacking-from-scratch/) on Udemy. The course covers Python scripting and its application in ethical hacking, network security, and more.
