# ArkKVM Open Source
ArkKVM is a compact IP-KVM platform designed to provide BIOS-to-desktop remote access through a standard web browser.  
The platform integrates video capture, USB device emulation, audio forwarding, remote power control, networking, and cloud connectivity into a single device, making it suitable for homelabs, self-hosting, remote administration, edge deployments, and embedded systems.

⸻

## Why Open Source?
ArkKVM is open sourced primarily for:  
	•	Transparency  
	•	Security review  
	•	Long-term software availability  
The goal of this effort is not to build a community-driven development model, but to ensure users can audit, understand, and continue using their devices independently of the company.  
We believe users should be able to inspect how their devices work, review security-sensitive components, and maintain access to the software that powers their hardware.

⸻

## Project Structure
The ArkKVM software stack is organized into several repositories:  
ArkKVM  
│  
├── ArkKVM OS  
│   Embedded Linux platform (Buildroot, Linux kernel, board support)  
│  
├── arkkvm-app  
│   Device-side system software  
│  
├── arkkvm-display-app  
│   On-device small-screen UI  
│  
├── arkkvm-app-frontend  
│   Browser frontend  
│  
└── arkkvm-cloud  
    Cloud services
### Repositories
|Repository|Description|
|:------------------|:------------------|
| **arkkvm-system** | ArkKVM OS |
| **arkkvm-app** | Main device-side system software running on ArkKVM hardware |
| **crates/usb_devices** | USB gadget sidecar (arkkvm_usb) within arkkvm-app |
| **arkkvm-usb-mic** | Virtual microphone audio playback (arkkvm_mic) |
| **arkkvm-display-app** | On-device small-screen UI (LVGL) for the built-in touchscreen |
| **arkkvm-app-frontend** | Browser frontend used by both device-local and cloud workflows |
| **arkkvm-cloud** | Cloud services supporting remote access and device connectivity |




⸻

## Open Source Status
Currently available:  
	•	✅  arkkvm-system  
    •	✅  arkkvm-app  
    •	✅  crates/usb_devices  
    •	✅  arkkvm-usb-mic  
	•	✅  arkkvm-display-app  
	•	✅  arkkvm-app-frontend  
	•	✅  arkkvm-cloud  

Repository availability may evolve over time as components are prepared for public release.

⸻

## Security
Security is important for any remote management platform.  
If you discover a security vulnerability, please do not report it through public GitHub issues.  
Instead, contact:  
contact@arkkvm.com  
We aim to:  
	•	Acknowledge reports within 72 hours  
	•	Work with researchers toward responsible disclosure  
	•	Credit reporters where appropriate and requested  

⸻

## License
Unless otherwise noted, ArkKVM open-source repositories are licensed under the **GNU General Public License v2.0 or later (GPL-2.0-or-later)**.

Some repositories may include or depend on third-party components that are distributed under their own licenses or are subject to additional redistribution restrictions, such as vendor SDKs, binary firmware, or proprietary libraries.

Please refer to the `LICENSE` file and accompanying notices in each repository for repository-specific licensing information.

⸻

## Community and Support
ArkKVM is currently maintained by a small engineering team.  
We welcome:  
	•	Bug reports  
	•	Security reports  
	•	Documentation feedback  
	•	Technical discussions  

Due to limited engineering resources:  
	•	Pull requests may not receive immediate review  
	•	Some repositories may not accept external contributions  
	•	Project direction and architecture remain managed by the core ArkKVM team  
Our current priority is delivering reliable software, maintaining product quality, and ensuring long-term support for existing users.

⸻

## Learn More
	•	Website: https://www.arkkvm.com  
	•	Documentation: https://docs.arkkvm.com  
	•	GitHub Organization: https://github.com/arkkvm  
Thank you for your interest in ArkKVM and for supporting open, transparent infrastructure software.
