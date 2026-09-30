# Awesome sing-box [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of clients, GUIs, panels, rule sets, and tools built on [sing-box](https://github.com/SagerNet/sing-box), the universal proxy platform.

sing-box supports Shadowsocks, VLESS, VMess, Trojan, WireGuard, Hysteria2, TUIC, and more, with powerful route rules and binary rule sets (`.srs`). This list collects the ecosystem around it. Entries are ordered roughly by GitHub stars or App Store presence; open-source unless marked.

Contributions welcome, see [CONTRIBUTING.md](CONTRIBUTING.md).

## Contents

- [Core](#core)
- [Official clients](#official-clients)
- [Desktop clients and GUIs](#desktop-clients-and-guis)
- [Mobile and Apple-platform clients](#mobile-and-apple-platform-clients)
- [Server panels and install scripts](#server-panels-and-install-scripts)
- [Rule sets and geodata](#rule-sets-and-geodata)
- [Subscription and config tools](#subscription-and-config-tools)

## Core

- [SagerNet/sing-box](https://github.com/SagerNet/sing-box) - The universal proxy platform itself. CLI, library, and the engine behind everything below.
- [Documentation](https://sing-box.sagernet.org/) - Official docs: configuration schema, route rules, rule-set format.
- [sing-box-lx](https://github.com/Leadaxe/sing-box-lx) - Client-side sing-box fork kept in sync with upstream stable; adds XHTTP transport, AmneziaWG 2.0/3.x, a MASQUE (CONNECT-IP) outbound, and VLESS post-quantum encryption, each isolated behind build tags or separate files. Ships as a drop-in `sing-box` binary.

## Official clients

Maintained by SagerNet, using the sing-box core directly:

- [sing-box for iOS (SFI)](https://apps.apple.com/us/app/sing-box-vt/id6673731168) - Official iOS client.
- [sing-box for macOS (SFM)](https://sing-box.sagernet.org/installation/clients/sfm/) - Official macOS client (App Store and standalone).
- [sing-box for Android (SFA)](https://github.com/SagerNet/sing-box-for-android) - Official Android client.
- [sing-box for Apple tvOS (SFT)](https://sing-box.sagernet.org/installation/clients/sft/) - Official Apple TV client.

## Desktop clients and GUIs

- [v2rayN](https://github.com/2dust/v2rayN) - Windows/Linux/macOS GUI supporting both Xray and sing-box cores.
- [nekoray](https://github.com/MatsuriDayo/nekoray) - Qt cross-platform GUI with sing-box backend. **No longer maintained**; kept here because many guides still reference it.
- [ShellCrash](https://github.com/juewuy/ShellCrash) - Run sing-box or mihomo as a client from a shell; popular on routers.
- [GUI.for.SingBox](https://github.com/GUI-for-Cores/GUI.for.SingBox) - Modern, lightweight desktop GUI built with Wails (Go) and Vue 3.
- [Throne](https://github.com/throneproj/Throne) - Cross-platform GUI proxy utility powered by sing-box; a maintained successor in the nekoray lineage.
- [singbox-launcher](https://github.com/Leadaxe/singbox-launcher) - Windows/macOS/Linux GUI for sing-box, bundled with the sing-box-lx core; multi-subscription management, visual routing configurator, per-process traffic profiler, and remote management of cores on routers or VPS.

## Mobile and Apple-platform clients

- [Hiddify](https://github.com/hiddify/hiddify-app) - Multi-platform auto-proxy client supporting sing-box, Xray, TUIC, Hysteria, Reality, Trojan, and more.
- [NekoBox for Android](https://github.com/MatsuriDayo/NekoBoxForAndroid) - sing-box based universal proxy toolchain for Android.
- [Karing](https://github.com/KaringX/karing) - Simple and powerful proxy utility with support for Clash and sing-box routing rules; iOS, Android, Windows, macOS.
- [Traveler's VPN](https://travelersvpn.com/) - Commercial, closed-source iOS/iPadOS/macOS client built on the sing-box core; automatic split-tunnel travel routing over user-supplied Outline/Shadowsocks, WireGuard, or Trojan servers, driven by `.srs` rule sets. *(Maintained by this list's author; see disclosure below.)*

## Server panels and install scripts

- [v2ray-agent](https://github.com/mack-a/v2ray-agent) - Eight-in-one install script covering Xray, TUIC, Hysteria2, and sing-box.
- [s-ui](https://github.com/alireza0/s-ui) - Advanced web panel built for SagerNet/sing-box.
- [sing-box-yg](https://github.com/yonggekkk/sing-box-yg) - Feature-rich sing-box VPS install script (Chinese).
- [Hiddify-Manager](https://github.com/hiddify/Hiddify-Manager) - Multi-user anti-filtering server panel supporting sing-box protocols.
- [fscarmen/sing-box](https://github.com/fscarmen/sing-box) - One-key multi-protocol sing-box deployment script (Chinese).

## Rule sets and geodata

- [SagerNet/sing-geosite](https://github.com/SagerNet/sing-geosite) - Official geosite data compiled to binary `.srs` rule sets (`rule-set` branch).
- [SagerNet/sing-geoip](https://github.com/SagerNet/sing-geoip) - Official GeoIP data as `.srs` rule sets (`rule-set` branch).
- [Loyalsoldier/geoip](https://github.com/Loyalsoldier/geoip) - Enhanced customizable GeoIP files, including sing-box formats.

## Subscription and config tools

- [sublink-worker](https://github.com/7Sageer/sublink-worker) - Cloudflare Worker that converts subscriptions for multiple clients, including sing-box.
- [serenity](https://github.com/SagerNet/serenity) - Official sing-box configuration generator server.

## Disclosure

This list is maintained by the developer of [Traveler's VPN](https://travelersvpn.com/), one of the entries above. Every other entry is included on merit and ordered by adoption; corrections and additions are welcome and are held to the same standard regardless of origin.

## License

[CC0 1.0](LICENSE) - public domain.
