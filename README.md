# Who Is Grooming Your Kids?

This is a free, router-level guide. It helps block adult content, monitor devices, and enforce parental controls on your home network. No paid subscriptions. No apps. You do not need to touch anyone else's devices.

---

## The Story Behind This Guide

It started with a suspicion.

A parent notices changes in their child's behavior. The child becomes quieter, more withdrawn, and secretive about their phone. The router's log shows a device connecting at 1am, then again at 4am, and then again the next night. An unidentified device with no hostname and a random MAC address is active late at night.

Sound familiar?

This scenario is common. It happens in countless homes worldwide, including places where conversations about online safety have not kept pace with the technology now everywhere.

---

## The Threat Is Real, and It Is Growing

* 90% of boys and 60% of girls are exposed to online pornography before the age of 18.
* Apps like VidMate and Snaptube, distributed outside official app stores, bundle adult content aggregators, hidden adware, and, in documented cases, spyware. They are built specifically to bypass platform content policies.
* DNS-over-HTTPS and DNS-over-TLS, protocols that encrypt and secure DNS queries, are built into modern browsers and apps. This means that simply changing your router's DNS settings isn't enough on its own.
* A child who knows what they are doing can defeat most basic parental controls in under five minutes using a free VPN app, which hides their online activity from parental controls, or a sideloaded browser, a web browser installed from outside the usual app store that can bypass restrictions.

Exposure to inappropriate content is not the only risk. There are also concerns about normalizing such content for young people, the grooming potential of certain platforms, and unwanted data collection on devices used for homework.

---

## Why Most Families Are Not Protected

The gap is not a lack of caring. It is a lack of accessible information.

Most parental control guides assume a premium router, a paid subscription, or deep technical knowledge. Most families, especially in developing regions where fibre internet is still relatively new, are using ISP-provided routers they have never logged into, set to default settings, with no filtering whatsoever.

The ISP installs the router and leaves. An unfiltered pipe into the global internet sits open in your home, 24 hours a day, accessible to anyone on your WiFi.

## This simple guide exists to close that gap  for free.

---

## What This Guide Covers

| Layer | Tool | Purpose |
|---|---|---|
| DNS filtering | OpenDNS Home (free) | Block adult content, malware, phishing network-wide |
| DNS bypass prevention | Router IP Filter | Block DoT (port 853) and DoH server IPs |
| IP auto-update | Router DDNS | Keep OpenDNS pointed at your correct home IP |
| Device identification | Router DHCP table | Map MAC addresses to devices and users |
| Time restrictions | Router Parental Controls | Restrict internet hours per device |
| Activity logging | OpenDNS Dashboard | Audit DNS queries and blocked attempts |

No paid subscriptions. No apps installed on devices. About 45 minutes of setup.

---

## Quick Start

👉 **[Read the Full Step-by-Step Guide →](GUIDE.md)**

| Step | What You'll Do |
|---|---|
| [Identify Devices](GUIDE.md#step-1--identify-all-devices-on-your-network) | Build a device registry from your router's DHCP table |
| [Set Up OpenDNS](GUIDE.md#step-2--set-up-opendns-home) | Create your free account and configure content filtering |
| [Configure Router DNS](GUIDE.md#step-3--configure-your-router-dns) | Point your router and all devices to OpenDNS |
| [Block Bypass Methods](GUIDE.md#step-4--block-dns-bypass-methods) | Block DoT and DoH at the firewall level |
| [Set Up DDNS](GUIDE.md#step-5--set-up-ddns-for-ip-auto-update) | Keep OpenDNS updated when your IP changes |
| [Block Sideloaded Apps](GUIDE.md#step-6--block-sideloaded-app-download-sites) | Block VidMate and similar APK sources |
| [Time Restrictions](GUIDE.md#step-7--set-time-based-restrictions-per-device) | Set internet curfews per device |

---

## Prerequisites

- Access to your router admin panel , usually `http://192.168.100.1` or `http://192.168.1.1`
- A free [OpenDNS Home](https://www.opendns.com/home-internet-security/) account
- Your router admin credentials (usually printed on the router sticker)

---

## Hardware Tested On

- **Router:** Huawei HG8546M-RMS (EchoLife GPON Terminal CLASS B+)
- **Connection:** PPPoE over GPON fibre
- **Applicable to:** Most ISP-provided home routers with a Security/Firewall section

---

## Limitations

- Mobile data (4G/5G) bypasses all WiFi controls ,carrier-level restrictions are needed for that
- Advanced VPNs with non-standard server IPs may still work
- This is a strong defensive layer, not a substitute for open conversation with your children

---

## Contributing

Found an error? Have a fix for a different router brand or ISP configuration?

**Contributions and corrections are welcome.** Please open an issue or submit a pull request.
This guide is intended to grow into a community resource particularly across Africa and other
regions where practical home network security documentation is scarce.

---

## Acknowledgements

This guide was developed through a real home network audit and security hardening exercise.
The technical writeup and documentation were produced in conjunction with
**[Anthropic's Claude AI](https://www.anthropic.com)** as a collaborative research and writing tool.

The implementation, testing, troubleshooting, and real-world context are human. The polish is shared.

---
---

<div align="center">

*Built by a guardian , for other guardians/parents.*
*The router in your hallway is the most powerful parental control you already own ,
you just need to know how to use it.*

</div>

