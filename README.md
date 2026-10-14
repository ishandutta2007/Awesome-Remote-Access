# Awesome-Remote-Access

# Top Remote Access Tools Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Remote Desktop Control, Game Streaming & Self-Hosted Access Infrastructure*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Remote Access**. These tools let you control a computer from anywhere — whether for tech support, remote work, or streaming games from your own hardware — with options ranging from polished commercial services to fully self-hosted open-source alternatives that keep your data on your own infrastructure.

**Examples** include Moonlight, Sunshine, Parsec, RustDesk, AnyDesk, Zoho Assist, TeamViewer, Splashtop, Chrome Remote Desktop, and Microsoft Remote Desktop (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom relay servers, and transparent remote access — ideal for privacy-conscious users, homelab enthusiasts, and teams avoiding commercial-use pop-ups and subscription fees.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Parsec](https://parsec.app/)**  
  Low-latency remote desktop and game streaming service. Free for personal use with paid Warp tier for teams. Easier setup than self-hosted alternatives and strong for co-op and remote collaboration. Closed-source, with advanced features like 4:4:4 color mode and virtual displays behind the paid tier .

- **[AnyDesk](https://anydesk.com/)**  
  Popular remote desktop software known for speed and simplicity. Uses proprietary DeskRT codec for high frame rates and low latency even on poor connections. Free for personal use; commercial use may trigger pop-ups. Strong cross-platform support including FreeBSD, Raspberry Pi, and ChromeOS viewing .

- **[TeamViewer](https://www.teamviewer.com/)**  
  Long-standing remote access standard with robust features including file transfer, remote printing, multi-monitor support, and session recording. Free version has become increasingly restrictive with commercial-use detection pop-ups .

- **[Zoho Assist](https://www.zoho.com/assist/)**  
  Cloud-based remote support and access software with unattended access, screen sharing, and file transfer. Integrated with Zoho's business suite.

- **[Splashtop](https://www.splashtop.com/)**  
  Remote access and support software with high-performance streaming, file transfer, and multi-monitor support.

- **[Chrome Remote Desktop](https://remotedesktop.google.com/)**  
  Free, browser-based remote access tied to your Google account. Simple setup and works in a pinch, but limited file transfer, clunky multi-monitor support, and designed for basic tasks only .

- **[Microsoft Remote Desktop](https://apps.microsoft.com/detail/9wzdncrfj3ps)**  
  Native RDP client for Windows, macOS, iOS, and Android. Connects to Windows Remote Desktop Services and Azure Virtual Desktop.

## Open-Source GitHub Projects

- **[Sunshine](https://github.com/LizardByte/Sunshine)**  
  **The leading open-source game streaming server** for Moonlight clients. Hardware-accelerated encoding for AMD, Intel, and Nvidia GPUs with low latency. Web UI for configuration and PIN-based pairing. Available for Linux, Windows, macOS, and FreeBSD. Apache 2.0 licensed. Runs on your own hardware, streaming your full game library with no catalog restrictions .

- **[Moonlight](https://github.com/moonlight-stream/moonlight-qt)**  
  **The client for Sunshine** (and NVIDIA GameStream). Available on Windows, macOS, Linux, Android, iOS, ChromeOS, Raspberry Pi, and even Nintendo Switch and PlayStation Vita with homebrew. PIN-based pairing, hardware-accelerated decoding, and multi-controller support. The recommended client for self-hosted game streaming .

- **[RustDesk](https://github.com/rustdesk/rustdesk)**  
  **The leading open-source TeamViewer/AnyDesk alternative.** Built in Rust for performance and low latency. Features file transfer, chat, session recording, and clipboard sync. Free for personal and commercial use. **Self-hostable** via Docker for full data privacy and faster connections. Open-source codebase means anyone can audit for backdoors. Supports Windows, macOS, Linux (including Wayland multi-scaled displays), Android, and iOS as controller. AGPL-3.0 licensed .

- **[Apache Guacamole](https://github.com/apache/guacamole-server)**  
  **Clientless remote desktop gateway.** Supports VNC, RDP, and SSH through an HTML5 web application — no plugins or client software required. Access your machines from any web browser. Built on a well-documented API for integration into other applications. Apache 2.0 licensed .

- **[MeshCentral](https://github.com/Ylianst/MeshCentral)**  
  **Open-source remote management for fleets of machines.** Node.js server pairs with a lightweight agent for Windows, macOS, and Linux. Browser console provides remote desktop, terminal, file manager, system info, and scriptable batch actions across your fleet. Two-factor auth, LDAP, and per-device permissions included. Best for managing more than five machines .

- **[ScottiBYTE Assist](https://github.com/scottibyte/scottibyte-assist-server)**  
  **Open-source attended remote assistance** for Windows and Linux. Designed as an alternative to TeamViewer and AnyDesk, but focused on **customer-initiated temporary support sessions** rather than persistent unattended access. Six-digit support codes, customer approval before access, individually authorized provider computers. Self-hosted server with client download portal. Docker deployment with SQLite storage. Native Windows and Ubuntu clients with X11 and Wayland support .

- **[Remotely](https://github.com/immense/Remotely)**  
  **Open-source on-demand support tool** for MSPs. .NET 8 and Blazor-based server runs in Docker. Technician logs in via browser, user downloads a small executable, and shares a six-digit code. Provides remote control, remote scripting (PowerShell/Bash), clipboard and file transfer. GPLv3 licensed. Best for on-demand support sessions where the user won't install a permanent agent .

- **[Rabbit Remote Control](https://github.com/KangLin/RabbitRemoteControl)**  
  **Cross-platform, multi-protocol remote control software.** Supports VNC, RDP, Terminal, SSH, TELNET, serial port, file transfer (FTP, SFTP), player, and network tools. Available for Windows, Unix/Linux, Android, macOS. Aims to be simple, convenient, secure, and easy to use .

- **[Nexterm](https://github.com/gnmyt/Nexterm)**  
  **Open-source server management software** for SSH, VNC, and RDP. Features SFTP file management, Docker deployment, Proxmox LXC/QEMU management, two-factor authentication, OIDC SSO, and organization-based user/server separation. MIT licensed .

- **[TigerVNC](https://github.com/TigerVNC/tigervnc)**  
  **Classic, reliable VNC** implementation. Boring in the best way — when you need plain VNC and nothing more. Cross-platform, actively maintained .

### Additional Strong Open-Source Options

- **Firezone** — Secure remote access gateway supporting WireGuard with Web GUI, 1-line install, MFA, and SSO .
- **Warpgate** — Smart SSH and HTTPS bastion that works with any SSH client. Rust/Docker .
- **ShellHub** — Modern SSH server for remotely accessing Linux devices via CLI or web UI .
- **Sshwifty** — SSH and Telnet connector made for the web. AGPL-3.0 .
- **Termix** — Clientless web-based server management with SSH terminal, tunneling, and file editing .

**Frameworks for building custom systems**: Combine **Sunshine + Moonlight** for self-hosted game streaming, **RustDesk** for general remote desktop with self-hosting, **Apache Guacamole** for browser-based clientless access, **MeshCentral** for fleet management, and **ScottiBYTE Assist** or **Remotely** for attended support sessions to build a complete self-hosted remote access stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Remote access tools must comply with data protection regulations (GDPR, CCPA), computer fraud laws, and organizational security policies. Unauthorized access to computer systems is illegal.
- Self-hosted open-source solutions require proper security hardening, reverse proxy configuration, and network security. Exposing remote access services directly to the internet without protection is dangerous .
