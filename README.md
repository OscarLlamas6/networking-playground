# networking-playground

Laboratorio personal de autoestudio de networking — desde fundamentos de red y CCNA hasta BGP avanzado, eBPF, SRv6, QUIC e Iroh. Diseñado para 12-24 meses de estudio progresivo. La numeración de carpetas ES el mapa de aprendizaje.

## Leyenda de niveles

- 🟢 Básico (CCNA 1)
- 🟡 Intermedio (CCNA 2-3)
- 🔴 Avanzado
- 🔵 Expert / Especialista

---

## Ruta de aprendizaje recomendada

```
Meses 1-3:   01 → 02 → 03 → 04 → 05 → 30   (fundamentos + herramientas de diagnóstico)
Meses 4-6:   06 → 07 → 08 → 13 → 15 → 23   (routing + protocolos + hardware + TCP/DNS)
Meses 7-9:   09 → 10 → 11 → 12 → 16 → 22   (BGP + internet architecture + NAT + WiFi)
Meses 10-12: 17 → 18 → 19 → 20 → 21         (VPNs + WireGuard + seguridad + cloud)
Meses 13-16: 14 → 24 → 25 → 26               (QUIC + eBPF + SRv6 + K8s networking)
Meses 17-20: 27 → 28 → 29 → 31 → 32         (Iroh + SDN + observabilidad + certs)
Meses 21-24: 33 + temas nuevos que vayan surgiendo
```

Categorías 03 (IPv6) y 07 (MPLS) se intercalan naturalmente en meses 4-9.

---

## Índice de categorías

| # | Categoría | Nivel | Descripción |
|---|-----------|-------|-------------|
| [01](01-fundamentos-de-red/) | Fundamentos de Red | 🟢 | Conceptos base de networking: modelo OSI, TCP/IP, medios físicos, dispositivos de red y protocolos de capa 2. |
| [02](02-direccionamiento-ipv4/) | Direccionamiento IPv4 | 🟢 | Estructura del espacio de direcciones IPv4, subnetting, CIDR, VLSM y servicios DHCP. |
| [03](03-ipv6/) | IPv6 | 🟢🟡 | Protocolo IPv6: estructura, tipos de dirección, NDP, SLAAC, DHCPv6, transición desde IPv4 y uso en BGP. |
| [04](04-switching-y-lan/) | Switching y LAN | 🟢🟡 | Tecnologías de switching de capa 2: VLANs, STP, EtherChannel, FHRP y tecnologías de overlay como VXLAN. |
| [05](05-routing-fundamentos/) | Routing Fundamentos | 🟢 | Conceptos fundamentales de routing: tablas de rutas, rutas estáticas, flotantes, default y protocolo RIP. |
| [06](06-routing-protocolos-avanzados/) | Routing Protocolos Avanzados | 🟡 | Protocolos de routing dinámico avanzados: OSPF uni y multiárea, OSPFv3, EIGRP, redistribución y filtrado. |
| [07](07-mpls/) | MPLS | 🟡🔴 | Multiprotocol Label Switching: etiquetas, LDP, RSVP-TE, L3VPN, L2VPN y comparación con SRv6. |
| [08](08-wan-y-sd-wan/) | WAN y SD-WAN | 🟡🔴 | Tecnologías WAN clásicas y modernas, SD-WAN con Cisco Viptela, Meraki y VMware VeloCloud. |
| [09](09-bgp-fundamentos/) | BGP Fundamentos | 🟡🔴 | BGP desde cero: AS, eBGP/iBGP, atributos, comunidades, route reflectors y confederaciones. |
| [10](10-bgp-avanzado/) | BGP Avanzado | 🔴🔵 | Aspectos avanzados de BGP: RPKI, BGPsec, Flowspec, Graceful Restart, Add-Paths y traffic engineering. |
| [11](11-internet-architecture/) | Internet Architecture | 🔴 | Arquitectura de Internet: jerarquía de ISPs, peering, transit, IXPs, multihoming y registros de recursos. |
| [12](12-anycast-y-ddos/) | Anycast y DDoS | 🔴🔵 | Routing anycast con BGP, ECMP, mitigación de DDoS con RTBH, Flowspec y scrubbing centers. |
| [13](13-tcp-udp-profundo/) | TCP/UDP Profundo | 🟡🔴 | Análisis profundo de TCP y UDP: handshake, control de flujo, congestión, TLS 1.2/1.3, tcpdump y Wireshark. |
| [14](14-quic-y-http3/) | QUIC y HTTP/3 | 🔴🔵 | Protocolo QUIC: multiplexación, 0-RTT, migración de conexión, BBR v2, HTTP/3 y implementaciones en Rust. |
| [15](15-dns/) | DNS | 🟢🟡🔴 | Sistema de Nombres de Dominio: resolución, tipos de registros, DNSSEC, DNS sobre TLS/HTTPS/QUIC y servidores. |
| [16](16-nat-y-traversal/) | NAT y Traversal | 🟡🔴 | NAT (SNAT, DNAT, CGNAT), tipos de NAT, traversal con STUN/TURN/ICE y UDP hole punching. |
| [17](17-vpns-y-tunneling/) | VPNs y Tunneling | 🟡🔴 | Tecnologías VPN: IPSec, IKEv2, GRE, SSL/TLS VPN, overlays, VXLAN, GENEVE y OpenVPN. |
| [18](18-wireguard/) | WireGuard | 🔴 | Protocolo WireGuard: cryptokey routing, handshake, Linux, containers, Kubernetes y herramientas derivadas. |
| [19](19-firewalls-y-ngfw/) | Firewalls y NGFW | 🟡🔴 | Firewalls stateful/stateless, NGFW, IDS/IPS, plataformas Cisco/Palo Alto/Fortigate y nftables/iptables. |
| [20](20-zero-trust-y-sase/) | Zero Trust y SASE | 🔴🔵 | Arquitecturas Zero Trust, ZTNA, SASE, SWG, CASB y soluciones Cloudflare Zero Trust, Zscaler, BeyondCorp. |
| [21](21-cloud-networking/) | Cloud Networking | 🔴 | Redes en la nube: VPC, subnets, peering, AWS/GCP/Azure networking avanzado, Direct Connect y BGP en cloud. |
| [22](22-wireless-y-wifi/) | Wireless y WiFi | 🟡🔴 | Estándares WiFi 802.11, frecuencias, WPA3, 802.1X, EAP, roaming, mesh y plataformas enterprise. |
| [23](23-hardware-y-plataformas/) | Hardware y Plataformas | 🟢🟡 | Plataformas de hardware y SO de red: Cisco IOS/IOS-XE/IOS-XR/NX-OS, Juniper JunOS, Arista EOS, GNS3, EVE-NG. |
| [24](24-ebpf-y-xdp/) | eBPF y XDP | 🔵 | eBPF y XDP: programabilidad del kernel Linux para networking, observabilidad y seguridad; DPDK y P4. |
| [25](25-srv6-y-segment-routing/) | SRv6 y Segment Routing | 🔵 | Segment Routing con MPLS y IPv6 (SRv6): SIDs, locators, behaviors, TE, VPNs y uso en 5G. |
| [26](26-kubernetes-networking-cni/) | Kubernetes Networking y CNI | 🔴🔵 | Networking en Kubernetes: modelo CNI, kube-proxy, Network Policies, Cilium, Calico, Flannel y benchmarks. |
| [27](27-iroh-y-p2p-moderno/) | Iroh y P2P Moderno | 🔵 | Protocolos P2P modernos: Iroh (n0-computer), DERP relay nodes, libp2p, Hypercore y DHT. |
| [28](28-sdn-y-automatizacion/) | SDN y Automatización | 🔴🔵 | Software Defined Networking: OpenFlow, controladores, NETCONF/YANG, gNMI, Ansible, Nornir y Terraform para redes. |
| [29](29-observabilidad-de-red/) | Observabilidad de Red | 🔴 | Herramientas de observabilidad: SNMP, NetFlow, sFlow, Prometheus, Grafana, ntopng, ELK y OpenTelemetry. |
| [30](30-herramientas-diagnostico/) | Herramientas de Diagnóstico | 🟢🔴 | Herramientas esenciales de diagnóstico: ping, traceroute, tcpdump, Wireshark, iperf3, nmap, dig y openssl. |
| [31](31-seguridad-de-red-avanzada/) | Seguridad de Red Avanzada | 🔴🔵 | Seguridad avanzada: RPKI, ROA, MANRS, tipos de DDoS, amplification attacks, BGP hijacking y forense de red. |
| [32](32-certificaciones-labs/) | Certificaciones y Labs | 🟢🟡🔴 | Roadmaps y labs para certificaciones: CCNA 200-301, CCNP Enterprise, JNCIA, AWS Advanced Networking, GCP Network Engineer. |
| [33](33-nuevas-tecnologias/) | Nuevas Tecnologías | 🔵 | Carpeta viva para tecnologías emergentes: WiFi 7, 5G/6G, TSN, computación in-network, AI networking y redes cuánticas. |

---

## Tabla comparativa

| Tema | Categoría | Nivel | Protocolo/Capa OSI | RFC / Estándar | Herramienta práctica | Estado |
|------|-----------|-------|-------------------|----------------|---------------------|--------|
| (completar a medida que se avanza) | — | — | — | — | — | pendiente |

---

## Progreso

### 01 - Fundamentos de Red 🟢

- [ ] 🟢 01-modelo-osi-7-capas
- [ ] 🟢 02-modelo-tcpip-4-capas
- [ ] 🟢 03-binario-hexadecimal-y-conversion
- [ ] 🟢 04-topologias-de-red
- [ ] 🟢 05-tipos-de-red-lan-man-wan
- [ ] 🟢 06-medios-fisicos-cobre-fibra-wireless
- [ ] 🟢 07-dispositivos-de-red-hubs-switches-routers
- [ ] 🟢 08-encapsulacion-y-pdu
- [ ] 🟢 09-ethernet-y-mac-addresses
- [ ] 🟢 10-arp-y-ndp

### 02 - Direccionamiento IPv4 🟢

- [ ] 🟢 01-estructura-ipv4
- [ ] 🟢 02-clases-de-red-abc
- [ ] 🟢 03-subnetting-y-mascara
- [ ] 🟢 04-cidr-y-vlsm
- [ ] 🟢 05-ip-publica-vs-privada-rfc1918
- [ ] 🟢 06-dhcp-fundamentos
- [ ] 🟢 07-dhcp-relay-y-server
- [ ] 🟢 08-supernetting

### 03 - IPv6 🟢🟡

- [ ] 🟢 01-por-que-ipv6
- [ ] 🟢 02-estructura-y-notacion
- [ ] 🟢 03-tipos-de-direcciones-uc-mc-anycast
- [ ] 🟡 04-ndp-neighbor-discovery
- [ ] 🟡 05-slaac-y-dhcpv6
- [ ] 🟡 06-dual-stack
- [ ] 🟡 07-tuneles-de-transicion-6to4-464xlat
- [ ] 🟡 08-ipv6-en-bgp

### 04 - Switching y LAN 🟢🟡

- [ ] 🟢 01-como-funciona-un-switch
- [ ] 🟢 02-vlans-y-trunking-802.1q
- [ ] 🟡 03-vtp-vlan-trunking-protocol
- [ ] 🟡 04-stp-spanning-tree
- [ ] 🟡 05-rstp-y-mstp
- [ ] 🟡 06-etherchannel-y-lacp-pagp
- [ ] 🟢 07-cdp-y-lldp
- [ ] 🟡 08-hsrp-vrrp-glbp
- [ ] 🟡 09-port-security
- [ ] 🟡 10-storm-control
- [ ] 🔴 11-vxlan-y-evpn

### 05 - Routing Fundamentos 🟢

- [ ] 🟢 01-como-funciona-un-router
- [ ] 🟢 02-routing-tables
- [ ] 🟢 03-rutas-estaticas
- [ ] 🟢 04-rutas-por-defecto
- [ ] 🟢 05-rutas-flotantes
- [ ] 🟢 06-rip-v2-legacy
- [ ] 🟢 07-redistribucion-basica
- [ ] 🟡 08-policy-based-routing

### 06 - Routing Protocolos Avanzados 🟡

- [ ] 🟡 01-ospf-fundamentos
- [ ] 🟡 02-ospf-areas-y-lsa
- [ ] 🟡 03-ospf-multiarea
- [ ] 🟡 04-ospfv3-para-ipv6
- [ ] 🟡 05-eigrp-fundamentos
- [ ] 🟡 06-eigrp-avanzado
- [ ] 🔴 07-redistribucion-entre-protocolos
- [ ] 🟡 08-route-filtering-y-prefix-lists
- [ ] 🔴 09-pbr-policy-based-routing-avanzado

### 07 - MPLS 🟡🔴

- [ ] 🟡 01-que-es-mpls
- [ ] 🟡 02-labels-y-label-switching
- [ ] 🟡 03-ldp-label-distribution-protocol
- [ ] 🔴 04-rsvp-traffic-engineering
- [ ] 🔴 05-mpls-vpn-l3vpn
- [ ] 🔴 06-mpls-vpn-l2vpn
- [ ] 🔴 07-mpls-vs-srv6

### 08 - WAN y SD-WAN 🟡🔴

- [ ] 🟡 01-tecnologias-wan-clasicas
- [ ] 🟡 02-ppp-y-frame-relay-legacy
- [ ] 🟡 03-metro-ethernet
- [ ] 🔴 04-sd-wan-conceptos
- [ ] 🔴 05-cisco-viptela-sdwan
- [ ] 🔴 06-meraki-sdwan
- [ ] 🔴 07-velocloud-vmware-sdwan
- [ ] 🔴 08-sdwan-vs-mpls

### 09 - BGP Fundamentos 🟡🔴

- [ ] 🟡 01-que-es-bgp-y-para-que
- [ ] 🟡 02-autonomous-systems-as
- [ ] 🟡 03-ebgp-vs-ibgp
- [ ] 🟡 04-establecimiento-de-sesion
- [ ] 🟡 05-estados-de-bgp
- [ ] 🟡 06-atributos-basicos-aspath-nexthop
- [ ] 🟡 07-nlri-y-prefix-advertisement
- [ ] 🟡 08-local-pref
- [ ] 🟡 09-med-multi-exit-discriminator
- [ ] 🟡 10-weight-cisco-specific
- [ ] 🔴 11-bgp-communities
- [ ] 🔴 12-route-reflectors
- [ ] 🔴 13-confederaciones-bgp

### 10 - BGP Avanzado 🔴🔵

- [ ] 🔴 01-rpki-y-roa
- [ ] 🔵 02-bgpsec
- [ ] 🔴 03-bgp-flowspec
- [ ] 🔴 04-bgp-graceful-restart
- [ ] 🔴 05-bgp-add-paths
- [ ] 🔴 06-bgp-extended-communities
- [ ] 🔴 07-bgp-large-communities
- [ ] 🔵 08-bgp-route-policies-avanzadas
- [ ] 🔵 09-bgp-traffic-engineering

### 11 - Internet Architecture 🔴

- [ ] 🔴 01-tier-1-tier-2-tier-3
- [ ] 🔴 02-peering-vs-transit
- [ ] 🔴 03-internet-exchange-points-ixp
- [ ] 🔴 04-peeringdb
- [ ] 🔴 05-route-servers
- [ ] 🔴 06-looking-glass
- [ ] 🔴 07-multihoming
- [ ] 🔴 08-provider-independent-pi-space
- [ ] 🔴 09-ripe-arin-lacnic-iana
- [ ] 🔴 10-internet-routing-registry-irr

### 12 - Anycast y DDoS 🔴🔵

- [ ] 🔴 01-anycast-fundamentos
- [ ] 🔴 02-anycast-con-bgp
- [ ] 🔴 03-ecmp-routing
- [ ] 🔴 04-anycast-dns
- [ ] 🔴 05-ddos-volumetrico-tipos
- [ ] 🔴 06-rtbh-remote-triggered-blackhole
- [ ] 🔵 07-flowspec-mitigacion
- [ ] 🔴 08-scrubbing-centers
- [ ] 🔴 09-ddos-protection-providers
- [ ] 🔵 10-anycast-cdn-y-cloudflare

### 13 - TCP/UDP Profundo 🟡🔴

- [ ] 🟡 01-tcp-3way-handshake
- [ ] 🟡 02-tcp-teardown
- [ ] 🟡 03-numeros-de-secuencia-y-ack
- [ ] 🟡 04-flow-control-y-sliding-window
- [ ] 🔴 05-congestion-control-cubic-bbr
- [ ] 🔴 06-head-of-line-blocking
- [ ] 🔴 07-tcp-fast-open
- [ ] 🟡 08-udp-fundamentos
- [ ] 🟡 09-udp-use-cases
- [ ] 🟡 10-tls-1-2-handshake
- [ ] 🔴 11-tls-1-3-handshake
- [ ] 🔴 12-sni-y-alpn
- [ ] 🟡 13-tcpdump-practico
- [ ] 🟡 14-wireshark-practico

### 14 - QUIC y HTTP/3 🔴🔵

- [ ] 🔴 01-por-que-quic
- [ ] 🔴 02-quic-vs-tcp
- [ ] 🔴 03-streams-multiplexados
- [ ] 🔴 04-0-rtt-resumption
- [ ] 🔴 05-connection-migration
- [ ] 🔴 06-loss-recovery
- [ ] 🔵 07-congestion-control-bbr-v2
- [ ] 🔵 08-quic-header-protection
- [ ] 🔴 09-http3-sobre-quic
- [ ] 🔵 10-webtransport
- [ ] 🔵 11-quinn-rust-implementacion
- [ ] 🔵 12-quiche-cloudflare
- [ ] 🔵 13-msquic-microsoft
- [ ] 🔴 14-quic-en-produccion

### 15 - DNS 🟢🟡🔴

- [ ] 🟢 01-como-funciona-dns
- [ ] 🟢 02-tipos-de-registros-a-aaaa-mx-cname
- [ ] 🟡 03-dns-autoritativo-vs-recursivo
- [ ] 🟡 04-dns-resolver-y-cache
- [ ] 🟡 05-zona-dns-y-delegacion
- [ ] 🟡 06-dns-inverso-ptr
- [ ] 🔴 07-dnssec
- [ ] 🔴 08-dns-over-tls-dot
- [ ] 🔴 09-dns-over-https-doh
- [ ] 🔴 10-dns-over-quic-doq
- [ ] 🔴 11-anycast-dns
- [ ] 🔴 12-dns-split-horizon
- [ ] 🟡 13-bind9-practico
- [ ] 🔴 14-coredns
- [ ] 🔴 15-unbound

### 16 - NAT y Traversal 🟡🔴

- [ ] 🟡 01-nat-fundamentos
- [ ] 🟡 02-snat-dnat-masquerade
- [ ] 🟡 03-full-cone-nat
- [ ] 🟡 04-symmetric-nat
- [ ] 🟡 05-port-restricted-nat
- [ ] 🔴 06-nat66-ipv6
- [ ] 🔴 07-cgnat-carrier-grade
- [ ] 🔴 08-stun
- [ ] 🔴 09-turn
- [ ] 🔴 10-ice-framework
- [ ] 🔴 11-udp-hole-punching
- [ ] 🔵 12-nat-traversal-con-quic
- [ ] 🟡 13-upnp-y-pmp

### 17 - VPNs y Tunneling 🟡🔴

- [ ] 🟡 01-ipsec-fundamentos
- [ ] 🟡 02-ikev1-vs-ikev2
- [ ] 🟡 03-ipsec-tunnel-vs-transport
- [ ] 🟡 04-gre-tunnels
- [ ] 🟡 05-gre-sobre-ipsec
- [ ] 🟡 06-l2tp
- [ ] 🟢 07-pptp-legacy
- [ ] 🟡 08-ssl-vpn-tls-vpn
- [ ] 🔴 09-overlay-vs-underlay
- [ ] 🔴 10-vxlan-fundamentos
- [ ] 🔴 11-vxlan-evpn
- [ ] 🔴 12-geneve
- [ ] 🟡 13-openvpn

### 18 - WireGuard 🔴

- [ ] 🔴 01-wireguard-conceptos
- [ ] 🔴 02-cryptokey-routing
- [ ] 🔴 03-wireguard-handshake
- [ ] 🔴 04-wireguard-linux-setup
- [ ] 🔴 05-wireguard-en-containers
- [ ] 🔴 06-wireguard-en-kubernetes
- [ ] 🔴 07-wg-quick-y-herramientas
- [ ] 🔴 08-boringtun-rust
- [ ] 🔴 09-netbird
- [ ] 🔴 10-tailscale-y-headscale
- [ ] 🔴 11-innernet

### 19 - Firewalls y NGFW 🟡🔴

- [ ] 🟡 01-tipos-de-firewall
- [ ] 🟡 02-stateful-vs-stateless
- [ ] 🟡 03-acls-y-packet-filtering
- [ ] 🔴 04-ngfw-conceptos
- [ ] 🔴 05-ips-ids-snort
- [ ] 🔴 06-suricata
- [ ] 🟡 07-cisco-asa
- [ ] 🔴 08-cisco-firepower-ftd
- [ ] 🔴 09-palo-alto-panos
- [ ] 🔴 10-fortigate
- [ ] 🟡 11-opnsense-pfsense
- [ ] 🟡 12-nftables-y-iptables
- [ ] 🟢 13-ufw

### 20 - Zero Trust y SASE 🔴🔵

- [ ] 🔴 01-zero-trust-conceptos
- [ ] 🔴 02-never-trust-always-verify
- [ ] 🔴 03-ztna-vs-vpn
- [ ] 🔴 04-swg-secure-web-gateway
- [ ] 🔴 05-casb
- [ ] 🔴 06-fwaas-firewall-as-a-service
- [ ] 🔵 07-sase-arquitectura
- [ ] 🔴 08-cloudflare-zero-trust
- [ ] 🔵 09-zscaler
- [ ] 🔵 10-netskope
- [ ] 🔴 11-identity-aware-proxy
- [ ] 🔵 12-beyondcorp

### 21 - Cloud Networking 🔴

- [ ] 🔴 01-vpc-architecture
- [ ] 🔴 02-subnets-publicas-privadas
- [ ] 🔴 03-vpc-peering
- [ ] 🔴 04-aws-transit-gateway
- [ ] 🔴 05-aws-direct-connect-bgp
- [ ] 🔴 06-aws-privatelink
- [ ] 🔴 07-gcp-cloud-interconnect
- [ ] 🔴 08-gcp-private-service-connect
- [ ] 🔴 09-azure-expressroute
- [ ] 🔴 10-azure-virtual-wan
- [ ] 🔵 11-multicloud-routing
- [ ] 🔴 12-cloud-bgp-consideraciones
- [ ] 🔴 13-security-groups-vs-nacls

### 22 - Wireless y WiFi 🟡🔴

- [ ] 🟡 01-802-11-fundamentos
- [ ] 🟡 02-frecuencias-24-5-6ghz
- [ ] 🟡 03-wifi-4-5-6-6e-7
- [ ] 🟡 04-wpa2-wpa3
- [ ] 🔴 05-802-1x-wireless
- [ ] 🔴 06-eap-peap-tls-wireless
- [ ] 🟡 07-captive-portals
- [ ] 🔴 08-roaming-y-handoff
- [ ] 🔴 09-mesh-networks
- [ ] 🟡 10-access-points-enterprise
- [ ] 🟡 11-cisco-meraki-wireless
- [ ] 🟡 12-ubiquiti-unifi

### 23 - Hardware y Plataformas 🟢🟡

- [ ] 🟢 01-cisco-ios-basico
- [ ] 🟡 02-cisco-ios-xe
- [ ] 🔴 03-cisco-ios-xr
- [ ] 🟡 04-cisco-nxos
- [ ] 🟡 05-cisco-asr-routers
- [ ] 🟢 06-cisco-isr-routers
- [ ] 🟢 07-cisco-catalyst-switches
- [ ] 🟡 08-cisco-nexus-switches
- [ ] 🟡 09-cisco-aironet-aps
- [ ] 🟡 10-juniper-junos-intro
- [ ] 🟡 11-arista-eos
- [ ] 🟢 12-gns3-lab-setup
- [ ] 🟡 13-eve-ng-lab-setup
- [ ] 🟢 14-packet-tracer

### 24 - eBPF y XDP 🔵

- [ ] 🔵 01-ebpf-fundamentos
- [ ] 🔵 02-bpf-maps
- [ ] 🔵 03-bpf-program-types
- [ ] 🔵 04-xdp-express-data-path
- [ ] 🔵 05-tc-hooks
- [ ] 🔵 06-socket-filter
- [ ] 🔵 07-bpftool
- [ ] 🔵 08-bpftrace
- [ ] 🔵 09-libbpf
- [ ] 🔵 10-ebpf-vs-iptables
- [ ] 🔵 11-ebpf-para-observabilidad
- [ ] 🔵 12-ebpf-para-seguridad
- [ ] 🔵 13-dpdk-data-plane-dev-kit
- [ ] 🔵 14-p4-programmable-dataplanes

### 25 - SRv6 y Segment Routing 🔵

- [ ] 🔵 01-segment-routing-conceptos
- [ ] 🔵 02-sr-mpls
- [ ] 🔵 03-srv6-fundamentos
- [ ] 🔵 04-srv6-sid-y-locator
- [ ] 🔵 05-srv6-behaviors
- [ ] 🔵 06-srv6-traffic-engineering
- [ ] 🔵 07-srv6-vpn-l3vpn-l2vpn
- [ ] 🔵 08-srv6-y-5g
- [ ] 🔵 09-srv6-vs-mpls-comparacion
- [ ] 🔵 10-srv6-en-linux

### 26 - Kubernetes Networking y CNI 🔴🔵

- [ ] 🔴 01-cni-model-fundamentos
- [ ] 🔴 02-kube-proxy-y-reemplazo
- [ ] 🔴 03-network-policies-l3-l4
- [ ] 🔵 04-network-policies-l7
- [ ] 🔵 05-cilium
- [ ] 🔵 06-cilium-bgp-control-plane
- [ ] 🔵 07-cilium-cluster-mesh
- [ ] 🔵 08-hubble-observabilidad
- [ ] 🔴 09-calico
- [ ] 🔵 10-calico-bgp-mode
- [ ] 🔴 11-flannel
- [ ] 🔴 12-weave-net
- [ ] 🔴 13-antrea
- [ ] 🔵 14-cni-comparison-benchmark

### 27 - Iroh y P2P Moderno 🔵

- [ ] 🔵 01-iroh-arquitectura
- [ ] 🔵 02-iroh-nodeid
- [ ] 🔵 03-iroh-direct-connections
- [ ] 🔵 04-iroh-derp-relay-nodes
- [ ] 🔵 05-iroh-blobs
- [ ] 🔵 06-iroh-docs-sync
- [ ] 🔵 07-nat-traversal-con-quic
- [ ] 🔵 08-libp2p
- [ ] 🔵 09-hypercore-protocol
- [ ] 🔵 10-dht-distributed-hash-table

### 28 - SDN y Automatización 🔴🔵

- [ ] 🔴 01-sdn-conceptos
- [ ] 🔴 02-openflow
- [ ] 🔴 03-opendaylight
- [ ] 🔴 04-onos
- [ ] 🔴 05-netconf-y-yang
- [ ] 🔴 06-restconf
- [ ] 🔵 07-grpc-y-gnmi
- [ ] 🔴 08-ansible-network-automation
- [ ] 🔴 09-napalm
- [ ] 🔴 10-nornir
- [ ] 🔴 11-terraform-network
- [ ] 🔵 12-pyats-genie
- [ ] 🔵 13-network-as-code

### 29 - Observabilidad de Red 🔴

- [ ] 🟡 01-snmp-v2-v3
- [ ] 🔴 02-netflow-y-ipfix
- [ ] 🔴 03-sflow
- [ ] 🔴 04-prometheus-network-exporters
- [ ] 🔴 05-grafana-dashboards-red
- [ ] 🔴 06-ntopng
- [ ] 🟡 07-zabbix
- [ ] 🔴 08-telegraf-y-influxdb
- [ ] 🔴 09-elk-para-red
- [ ] 🔵 10-opentelemetry-red
- [ ] 🟡 11-nmap-y-escaneo
- [ ] 🔴 12-flow-analysis

### 30 - Herramientas de Diagnóstico 🟢🔴

- [ ] 🟢 01-ping-y-icmp
- [ ] 🟢 02-traceroute-y-mtr
- [ ] 🟡 03-tcpdump
- [ ] 🔴 04-wireshark-avanzado
- [ ] 🟡 05-iperf3-y-throughput
- [ ] 🟡 06-netstat-y-ss
- [ ] 🟡 07-nmap
- [ ] 🟡 08-dig-y-drill
- [ ] 🟡 09-curl-y-http-debug
- [ ] 🔴 10-openssl-tls-debug
- [ ] 🟡 11-iptraf-y-nethogs
- [ ] 🟢 12-bmon-y-vnstat

### 31 - Seguridad de Red Avanzada 🔴🔵

- [ ] 🔴 01-rpki-fundamentos
- [ ] 🔴 02-roa-route-origin-authorization
- [ ] 🔵 03-bgpsec
- [ ] 🔴 04-manrs
- [ ] 🔴 05-ddos-tipos-y-vectores
- [ ] 🔴 06-amplification-attacks
- [ ] 🔴 07-spoofing-y-bcp38
- [ ] 🟡 08-arp-spoofing-y-mitigacion
- [ ] 🔴 09-dns-hijacking
- [ ] 🔴 10-bgp-hijacking-historico
- [ ] 🔵 11-network-forensics
- [ ] 🔴 12-honeypots-de-red

### 32 - Certificaciones y Labs 🟢🟡🔴

- [ ] 🟢 01-ccna-200-301-roadmap
- [ ] 🟢 02-ccna-1-labs
- [ ] 🟡 03-ccna-2-labs
- [ ] 🟡 04-ccna-3-labs
- [ ] 🔴 05-ccnp-enterprise-roadmap
- [ ] 🔴 06-ccnp-encor-labs
- [ ] 🟡 07-jncia-juniper
- [ ] 🔴 08-aws-advanced-networking
- [ ] 🔴 09-gcp-professional-network-engineer
- [ ] 🔴 10-cka-networking-foco

### 33 - Nuevas Tecnologías 🔵

- [ ] 🔵 01-wifi-7-802-11be
- [ ] 🔵 02-5g-y-network-slicing
- [ ] 🔵 03-6g-research
- [ ] 🔵 04-tsn-time-sensitive-networking
- [ ] 🔵 05-deterministic-networking
- [ ] 🔵 06-in-network-computing
- [ ] 🔵 07-ai-networking-autonomous
- [ ] 🔵 08-quantum-networking-intro
- [ ] 🔵 09-non-terrestrial-networks-ntn
- [ ] 🔵 10-placeholder-nuevo-tema

---

## Nota — 33 Nuevas Tecnologías

> Esta categoría es una carpeta viva. A medida que surjan nuevas tecnologías, protocolos o herramientas relevantes durante el período de estudio, se agregarán aquí como nuevas subcarpetas.

---

## Labs y simuladores recomendados

- **GNS3** — simulación de routers/switches reales
- **EVE-NG** — laboratorio de red empresarial
- **Packet Tracer** — Cisco oficial, gratis con cuenta NetAcad
- **Containerlab** — labs de red con containers
- **Kathará** — emulación de red basada en Docker
- **Mininet** — red virtualizada para SDN
