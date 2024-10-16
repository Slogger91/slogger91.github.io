# Overview
This configuration was created because I did not want to pay for Obsidian sync.

## High Level Overview
- Syncthing is running as an LXC ([[LXC - Syncthing]]) on [[Proxmox Host - PVE1]]
- It's IP Address is reserved in Pihole
	- The IP Address is 192.168.1.20.
	- The Web gui is running on port 8384
- The password is in Bitwarden - "Syncthing - GUI Password"
- LXC was built using this script (Search for SyncThing) - [Proxmox VE Helper-Scripts | Scripts for Streamlining Your Homelab with Proxmox VE (tteck.github.io)](https://tteck.github.io/Proxmox/)
## How to set up a new device to access Obsidian vault
1. Install Syncthing.
	- I used the windows installer for windows devices.
2. Share obsidian folder from Syncthing-LXC from PVE1.
	1. Can find this by going to Heimdall.
	2. ![[Pasted image 20240418183718.png]]
3. It will automatically start syncing.
4. In the meantime, download and install Obsidian.
5. Once installed, open an existing fault and open into the personal folder

Specific instructions can be found on the relevant websites.

- 