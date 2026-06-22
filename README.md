# 🌐 Portfolio Sieciowe Cisco (Laboratoria Packet Tracer)

---

## 🇵🇱 Wersja Polska 

### O projekcie
Niniejsze repozytorium stanowi moje profesjonalne portfolio z zakresu inżynierii teleinformatycznej, dokumentujące praktyczne umiejętności i postępy w nauce administracji sieciami komputerowymi. Znajdują się tu autorskie skrypty i scenariusze realizowane w środowisku **Cisco Packet Tracer**, które odwzorowują rzeczywiste konfiguracje urządzeń klasy Enterprise. Repozytorium jest regularnie rozbudowywane o nowe rozwiązania i protokoły sieciowe.

### Technologie i narzędzia
* **Symulator:** Cisco Packet Tracer 8.x
* **Sprzęt:** Routery Cisco ISR, Przełączniki Catalyst
* **Metoda konfiguracji:** Interfejs wiersza poleceń (CLI)
* **Status:** W trakcie rozwoju (regularne aktualizacje)

### Katalog Laboratoriów
* **[Lab 13] Tunelowanie GRE i Sieci VPN (Integracja LAN-WAN-LAN)**
  Projekt integracji odległych oddziałów przez publiczną sieć Internet za pomocą tuneli GRE (Generic Routing Encapsulation). Konfiguracja wirtualnych interfejsów tunelowych, hermetyzacja ruchu OSPF wewnątrz sieci VPN oraz równoległa implementacja NAT Overload dla dostępu do Internetu.
* **[Lab 12] Technologie WAN (PPP, Frame Relay)**
  Zarządzanie połączeniami szeregowymi w sieciach rozległych. Konwersja enkapsulacji do PPP wraz z bezpiecznym uwierzytelnianiem węzłów algorytmami CHAP. Projektowanie sieci NBMA przy użyciu technologii Frame Relay, w tym mapowanie adresów IP na kanały DLCI (wirtualne obwody PVC) oraz integracja środowiska wielodostępowego z routingiem OSPFv2.
* **[Lab 09-10] Trójwarstwowa Sieć Korporacyjna (HSRP, OSPFv2, DHCP & Extended ACLs)**
  Projekt kompletnej, odpornej na awarie infrastruktury w architekturze hierarchicznej (Access-Distribution-Core). Wdrożenie redundancji bramy HSRP z podziałem obciążenia na budynki, agregacji EtherChannel, centralnego serwera DHCP z przekazywaniem żądań (IP Helper) oraz restrykcyjnych, rozszerzonych list ACL w celu pełnej izolacji ruchu między podsieciami użytkowników.
* **[Lab 04] Kontrola Dostępu (Standard ACLs)**
  Wdrażanie standardowych list kontroli dostępu w celu zabezpieczenia dostępu zdalnego (Telnet), izolacji VLAN-ów oraz blokowania ruchu między oddziałami przy użyciu zoptymalizowanych masek wieloznacznych (wildcard masks).
* **[Lab 03] OSPFv2 Multi-Area**
  Konfiguracja routingu dynamicznego w strukturze wieloobszarowej (Backbone + obszary podrzędne). Skupienie na sumaryzacji tras na routerach ABR i optymalizacji tablic routingu.
* **[Lab 02] OSPFv2 Single-Area**
  Wdrożenie protokołu OSPF w jednym obszarze. Zadanie obejmowało ustawianie Router ID, pasywowanie interfejsów LAN oraz ręczną manipulację metryką (kosztem) łączy.
* **[Lab 01] Podstawy Infrastruktury Sieciowej**
  Kompleksowe powtórzenie: tworzenie VLAN-ów, Inter-VLAN routing (Router-on-a-Stick) oraz konfiguracja routera jako serwera DHCPv4.

---

## 🇪🇳 English Version 

### About the Project
This repository serves as my professional Teleinformatics engineering portfolio, documenting practical skills and progress in network administration. It features custom scripts and scenarios developed in **Cisco Packet Tracer**, mimicking real-world enterprise network configurations. The repository is regularly expanded with new network solutions and protocols.

### Tech Stack & Tools
* **Simulator:** Cisco Packet Tracer 8.x
* **Hardware:** Cisco ISR Routers, Catalyst Switches
* **Configuration Method:** Command Line Interface (CLI)
* **Status:** In Progress (Regular Updates)

### Project Catalog
* **[Lab 13] GRE Tunneling and VPNs (LAN-WAN-LAN Integration)**
  Integration of remote branches across the public Internet using Generic Routing Encapsulation (GRE) tunnels. Configuration of virtual tunnel interfaces, encapsulation of OSPF traffic within the VPN, and parallel implementation of NAT Overload for Internet access.
* **[Lab 12] WAN Technologies (PPP, Frame Relay)**
  Managing serial connections in Wide Area Networks. Conversion of encapsulation to PPP along with secure node authentication using CHAP. Designing an NBMA network using Frame Relay technology, including mapping IP addresses to DLCI channels (PVC virtual circuits) and integrating the multi-access environment with OSPFv2 routing.
* **[Lab 09-10] Three-Tier Enterprise Network (HSRP, OSPFv2, DHCP & Extended ACLs)**
  Design of a comprehensive, fault-tolerant network framework based on a hierarchical layout (Access-Distribution-Core). Features HSRP gateway redundancy with per-building load balancing, EtherChannel bundling, centralized DHCP with IP Helper relaying, and advanced Extended ACL execution to enforce user segment isolation.
* **[Lab 04] Access Control (Standard ACLs)**
  Implementing standard access control lists to secure remote management (Telnet), isolate VLANs, and block branch-to-branch traffic using optimized wildcard masks.
* **[Lab 03] OSPFv2 Multi-Area**
  Dynamic routing configuration in a multi-area structure (Backbone + subordinate areas). Focuses on route summarization at ABRs and routing table optimization.
* **[Lab 02] OSPFv2 Single-Area**
  Implementation of OSPFv2 within a single area. Tasks included setting Router IDs, configuring passive interfaces for LANs, and manual metric (cost) manipulation.
* **[Lab 01] Network Infrastructure Foundations**
  A comprehensive review covering VLAN creation, Inter-VLAN routing (Router-on-a-Stick), and configuring a router as a DHCPv4 server.