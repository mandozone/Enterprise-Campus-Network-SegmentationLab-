# Enterprise Campus Network Segmentation Lab

A Cisco Packet Tracer simulation of an enterprise campus network with **VLAN segmentation**, **802.1Q trunking**, **hierarchical switching**, and **Router-on-a-Stick inter-VLAN routing** across 18 departments — secured by a **nine-firewall ASA5505 perimeter**.

> **All 9 firewalls were configured by Romando Wright.**

## At a glance

| | |
|---|---|
| VLANs | 9 (VLAN 10–90) |
| Departments | 18 |
| Switches | 9 (1 core/distribution + 8 access) |
| Router | 1 (Router-on-a-Stick) |
| Firewalls | 9 × Cisco ASA5505 |
| Packet loss | 0% across inter-VLAN paths |
| Platform | Cisco Packet Tracer · Cisco IOS 15.1 · Kali Linux 2025.2 |

## Site

A polished, responsive web presentation of this lab lives in [`site/`](./site/). Open `site/index.html` in any browser, or serve it locally:

```bash
cd site
python3 -m http.server 8080
```

For GitHub Pages, point Pages at the `/site` directory.

## Primary file

`master network.pkt` — final completed topology with 18 departments, 9 switches, Router-on-a-Stick, and nine ASA5505 firewalls.

## Documentation

Full project writeup with topology evolution, VLAN plan, configuration, troubleshooting, and Phase 2 roadmap: [`enterprise-campus-network-lab (2).pdf`](./enterprise-campus-network-lab%20\(2\).pdf).
