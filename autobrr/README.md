# autobrr – Unraid Docker Template

This repository provides an **Unraid Docker template** for deploying and running autobrr on Unraid systems.

⚠️ This repository does NOT contain autobrr itself.  
It only provides a deployment template for Unraid.

All credit for autobrr goes to the original developers:

- Official GitHub: https://github.com/autobrr/autobrr  
- Official website: https://autobrr.com  

This template does not modify, redistribute, or bundle the autobrr software.

---

## About autobrr

autobrr is an automation tool that listens to torrent tracker IRC announce channels and forwards matched releases to download clients such as:

- qBittorrent  
- Transmission  
- Deluge  

It is commonly used for:

- Ratio building  
- Freeleech sniping  
- Instant grabbing of new releases  
- Advanced torrent automation workflows  

For documentation and support related to autobrr itself, please refer to the official project.

---

## What This Repository Provides

This repository includes:

- A ready-to-use Unraid XML Docker template  
- Proper `/config` mapping to Unraid appdata  
- WebUI configuration (default port 7474)  
- Standard Unraid environment variables (PUID, PGID, UMASK, TZ)  
- Clean integration into Unraid’s Docker system  

It allows easy deployment of autobrr without manual Docker configuration.

---

## Installation on Unraid

1. Add this repository as a template source in Unraid.
2. Select the autobrr template.
3. Configure:
   - Appdata path (default: `/mnt/user/appdata/autobrr`)
   - WebUI port (default: 7474)
   - Timezone
4. Deploy the container.
5. Access the WebUI at:
http://YOUR_UNRAID_IP:7474


At first launch, create your administrator account via the WebUI.

---

## Optional: Running Behind a VPN Container

If you use a VPN container such as Gluetun, you can attach autobrr to it using Unraid advanced Docker settings:

- Set **Network Type** to: `None`
- Add **Extra Parameters**:
--net=container:gluetun


This is optional and depends entirely on your setup.

---

## Disclaimer

This template:

- Is not affiliated with the autobrr project  
- Does not alter autobrr  
- Does not redistribute autobrr binaries  

For issues related to autobrr functionality, configuration, or bugs, please use the official project channels:

https://github.com/autobrr/autobrr

---

## Purpose of This Template

autobrr is not always available directly in Unraid Community Applications.

This repository provides a clean, reusable, and transparent way to deploy autobrr on Unraid systems while fully respecting the original project and its licensing.

---

## License

This repository contains only a Docker template file.

All autobrr software licensing and intellectual property belong to the original autobrr project and its developers.
