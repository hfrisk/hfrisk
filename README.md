# Greetings!

Hi, my name is Hunter Frisk. I'm a computer science and information technology student at Concordia University-Saint Paul. I'm currently working on a small personal website generator, and also have an interest in smart home systems and automation. 

## Technologies and Tools

### Programming Languages

* Lua/Luau :heart:
* Rust
* JavaScript/TypeScript
* Java
* Kotlin
* Python

### Tools

* Neovim :heart:
* VS Code
* IntelliJ
* Docker/Podman
* Nginx :heart:
* Asciidoc

## Currently working on

* **Unnamed Website Generator**: Existing static site generators like Jekyll and Antora are great, but I wanted to make my own for a personal website. Generates a homepage with links to markdown files, sorted by last-modified. 
* **Random Notification Daemons**: Small background scripts which randomly send me notifications on Windows and Linux. Both read from a directory of plaintext files, and serve their contents as system tray notifications. Re-writing these as a single cross-platform Rust application before I publish it.

## Homelab

I also run a small homelab centered around a converted desktop rig running Proxmox. 
* **The Monolith**: Proxmox, running an Ubuntu 24 VM as an OCI container host. Hosts
	* Jellyfin for listening to my music collection while on-the-go.
	* Home Assistant - a free and open-source alternative to proprietary smart home solutions.
	* A Samba server for network-attached file storage.
	* XBackBone for quickly sharing files without reliance on third-party servers.
	* A lightweight Minecraft server with automated stop-and-start based on activity. Runs the *Better Than Adventure* mod for Minecraft Beta 1.7.3, containerized in Podman via [itzg/docker-mine-craft-server](https://github.com/itzg/docker-minecraft-server). Surprisingly the most complex thing on the server, given:
	  * The outdated, highly-niche version of the game - no mc-router for Minecraft-aware routing and auto-scaling. No access to the Modflared mod to enable Cloudflare tunneling.
	  * The usage of rootless Podman over rootful Docker - no lazytainer for auto-scaling.
	  * Scheduled overnight map renders through Dynmap - so the container must be kept online at certain times of day, regardless of activity. 
	  * I don't actually like playing Minecraft very often. My friends are not very interested in this server. I don't know why I did this. 
	* Since Cloudflare tunneling does not work for Minecraft, I also have a high-speed VPN tunnel from my home to a VPS, protecting my home network. 
	I could probably do a series of write-ups on the Minecraft server and VPN tunnel. 
* **Raspberry Pi 3B+**: Runs HyperHDR to control ambient backlighting on my living room TV. Used to run Samba for network-attached file storage.
* **VPS**: A small, high-speed VPS rented from Racknerd. Hosts a VPN tunnel and reverse proxy, protecting my home network from intrusion.
I'll soon be adding two ESP32-backed displays: One to broadcast events from the systems' logs, and another for displaying system resource usage. 

## Other

I enjoy playing Old School RuneScape, reading manga, and watching movies. Some of my favorite filmmakers include Mamoru Oshii (*Stray Dog*, *Innocence*), James Cameron (*Terminator II*), Ridley Scott (*Alien*, *Prometheus*, *Blade Runner*), and David Lynch (*Twin Peaks*, *Lost Highway*).
