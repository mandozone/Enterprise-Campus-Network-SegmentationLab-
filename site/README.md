# Enterprise Campus Network Segmentation Lab — Static Site

A polished, responsive, single-page presentation of the **Enterprise Campus Network Segmentation Lab**: Cisco Packet Tracer simulation with VLAN segmentation, 802.1Q trunking, hierarchical switching, Router-on-a-Stick inter-VLAN routing, and a nine-firewall ASA5505 perimeter.

> **All 9 firewalls in this lab were configured by Romando Wright.**

## Deploy

This is a pure static site — no build step. Serve `site/` from any static host:

```bash
# Local preview
cd site
python3 -m http.server 8080
# then open http://localhost:8080
```

GitHub Pages: set the Pages source to `/site` on the `main` branch, or move the contents to the repo root.

## Files

- `index.html` — full single-page site
- `styles.css` — dark, responsive design system (Inter + JetBrains Mono)
- `assets/network-firewalls.jpeg` — master topology screenshot featuring all nine ASA5505 firewalls
- `assets/project-overview.jpeg` — project cover page

## Content

- Hero with project metrics (9 VLANs · 18 departments · 9 switches · 9 firewalls · 0% packet loss)
- Engineer-of-record section crediting Romando Wright for all nine firewalls
- Three-tier architecture diagram (Router → Core/Distribution → Access)
- Full VLAN segmentation table (VLAN 10–90 with subnets and gateways)
- Trunk, subinterface, and verification config snippets
- Nine firewall tiles + inline screenshot of the master topology
- Troubleshooting case studies (VID conflict, encapsulation order, DTP flap, native VLAN mismatch, topology rebuild)
- Skills demonstrated and Phase 2 security roadmap
