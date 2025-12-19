# Lab24-DMVPN
Configure a Dynamic Multipoint VPN (DMVPN Phase 1) architecture that allows multiple branch routers (spokes) to securely communicate with a central router (hub) using GRE multipoint tunnels and NHRP.

Topology Overview

Router 1 → DMVPN Hub

Router 2, 3, 4 → DMVPN Spokes

Each router has:

One LAN interface

One WAN interface (public network)

One Tunnel interface (DMVPN overlay)

OSPF is used as the routing protocol over the DMVPN tunnel.

Static routes are used to reach remote LANs via the tunnel.

NHRP dynamically maps tunnel IPs to public IPs.

Tunnel Network

DMVPN Tunnel Network: 11.11.11.0/24

Hub Tunnel IP: 11.11.11.1

Spokes Tunnel IPs: 11.11.11.2 – 11.11.11.4
