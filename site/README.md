# Enterprise Campus Network Segmentation Lab — Static Site

A polished, responsive, evidence-driven web presentation of the **Enterprise
Campus Network Segmentation Lab**: Cisco Packet Tracer simulation with VLAN
segmentation, 802.1Q trunking, hierarchical switching, Router-on-a-Stick
inter-VLAN routing, and a nine-firewall ASA5505 perimeter.

> **All 9 firewalls were configured by Romando Wright.**

## Deploy

Pure static site — no build step. Serve `site/` from any static host:

```bash
cd site
python3 -m http.server 8080
# → http://localhost:8080/
```

GitHub Pages: set the Pages source to `/site` on `main`, or move the contents to the repo root.

## Files

```
site/
├── index.html                      Recruiter-facing presentation page
├── styles.css                      Dark cybersec/network theme
├── README.md                       This file
└── assets/
    ├── topology-overview.jpg                 ← Group A: Topology evolution
    ├── topology-trunking.jpg
    ├── topology-hierarchical.jpg
    ├── topology-final-master.jpg
    ├── switch-vlan-creation.jpg              ← Group B: VLAN segmentation
    ├── switch-show-vlan-brief.jpg
    ├── router-subinterface-config.jpg        ← Group C: Router-on-a-Stick
    ├── router-encap-write-memory.jpg
    ├── router-show-ip-interface.jpg
    ├── ping-accounting.jpg                   ← Group D: Validation
    ├── network-firewalls-clean.jpeg          (firewall topology — clean crop)
    ├── network-firewalls.jpeg                (original phone source, linked from caption)
    ├── project-overview.jpeg                 (project cover)
    └── originals/                            Untouched source photos for every cropped derivative
```

## Content map

1. **Hero** — title, project stats, status pill
2. **TL;DR for Recruiters** — Problem / What I Built / How I Validated It / Why It Matters
3. **Engineer of Record** — Romando Wright credit + firewall scope bullets
4. **Tools &amp; Platforms** — chip grid
5. **Network Design** — three-tier ASCII diagram + layer/role/device table
6. **VLAN Segmentation Plan** — VLAN 10–90 table with names, subnets, gateways
7. **Router-on-a-Stick** — two config cards (router subinterfaces + switch trunk)
8. **Security Perimeter** — 9 firewall tiles + master topology screenshot
9. **Evidence** — four groups (A topology evolution · B VLANs · C routing · D validation), each photo with a clickable link to the original
10. **Skills Demonstrated** — capability table
11. **Recruiter Takeaway** — closing blockquote

## Image strategy

Each evidence image is a cropped, web-optimised derivative of a captured photo. The cropped JPGs live in `assets/`; the unedited source files are preserved in `assets/originals/` and linked from every figure caption via "View original source photo →".
