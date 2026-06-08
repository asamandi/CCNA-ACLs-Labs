# ACLs (Standard & Extended)

### configurations:

- Standard ACL
- Extended ACL
- Applying ACLs inbound/outbound
- Allowing some subnets
- Denying others
- Permit tests
- Block tests

### TOPOLOGY FOR ACL LAB:
- PC1 ---- R1 ---- R2 ---- Server

### Networks:
- LAN 1: 192.168.10.0/24 (PC1)
- Transit: 10.0.12.0/30 (R1–R2)
- Server LAN: 172.16.1.0/24 (Server)

### IP Addressing Plan

PC1:
- IP: 192.168.10.10
- GW: 192.168.10.1

R1:
- g0/0 = 192.168.10.1/24
- g0/1 = 10.0.12.1/30

R2:
- g0/0 = 10.0.12.2/30
- g0/1 = 172.16.1.1/24

Server:
- IP: 172.16.1.100
- GW: 172.16.1.1
