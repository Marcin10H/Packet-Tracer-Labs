# 🏢 Part 2: Implementacje Zaawansowanych Rozwiązań Teleinformatycznych (Advanced ICT Solutions)

---

## 🇵🇱 Wersja Polska

### O projekcie (Semestr Bieżący)
Niniejszy katalog dokumentuje zaawansowane scenariusze laboratoriów realizowane w ramach przedmiotu **Implementacje zaawansowanych rozwiązań teleinformatycznych**. Projekty skupiają się na budowie kompleksowych, odpornych na awarie sieci korporacyjnych (Enterprise) połączonych z segmentami rozległymi WAN, technologiami przełączania warstwy 2/3, zaawansowanym routingu oraz mechanizmach brzegowych i translacji adresów (NAT).

### Architektura i Konwencja Adresacji (Baza Projektowa)
Wszystkie tegoroczne laboratoria bazują na spójnej, w pełni unikalnej topologii bazowej (`exc_00_topology_preparation`), która integruje:
- **Segment Local Enterprise:** Prywatna pula adresowa klasy A (`10.50.0.0/16`) z podziałem na VLAN-y użytkowników (VLAN 10, 20), sieć IoT (VLAN 30) oraz administrację (VLAN 99), a także publiczny segment serwerowy (`85.100.10.0/27`).
- **Redundancja i Switchowanie:** Konfiguracja protokołu STP z optymalizacją korzeni (Root Primary/Secondary) oraz łącza agregowanego LACP (EtherChannel) na przełącznikach wielowarstwowych Cisco Catalyst 3650. Wdrożenie redundancji bramy domyślnej w architekturze HSRP (Hot Standby Router Protocol).
- **Segment WAN / Service Provider:** Sieć wielodostępowa oparta na chmurze Frame Relay (`SW_Cloud`) z mapowaniem DLCI oraz łączach szeregowych PPP.
- **Segmenty Zewnętrzne i Brzegowe:** Sieć publiczna (`PUBLIC` z serwerem Cloud w puli `198.51.100.0/26`) oraz sieć zdalna (`Remote` z operatorem NAT na routerie brzegowym obsługującym podsieć `172.25.10.0/24`).

### Katalog Laboratoriów / Modułów
- **[Lab 00] Przygotowanie Topologii i Adresacji Bazowej (`exc_00_topology_preparation`)**
  Inicjalizacja i pełne okablowanie demonstracyjnej topologii sieci rozległej. Zaprojektowanie i wdrożenie unikalnego schematu adresacji IPv4 (prywatnej i publicznej), konfiguracja subinterfejsów 802.1Q, serwerów DHCP na routerach bramowych, protokołu HSRP, statycznego mapowania Frame Relay oraz translacji NAT Overload dla sieci zdalnej.

---

## 🇪🇳 English Version

### About the Project (Current Semester)
This directory documents advanced laboratory scenarios implemented as part of the **Advanced ICT Solutions Implementation** course. The projects focus on building comprehensive, fault-tolerant Enterprise networks integrated with WAN wide-area segments, Layer 2/3 switching technologies, advanced routing, edge mechanisms, and Network Address Translation (NAT).

### Architecture & Addressing Convention (Base Topology)
All projects in this semester are built upon a consistent, fully custom base topology (`exc_00_topology_preparation`) integrating:
- **Local Enterprise Segment:** Private Class A address space (`10.50.0.0/16`) subdivided into user VLANs (VLAN 10, 20), IoT segment (VLAN 30), administration (VLAN 99), and a public server block (`85.100.10.0/27`).
- **Redundancy & Switching:** STP root optimization (Root Primary/Secondary) and LACP aggregated links (EtherChannel) on Cisco Catalyst 3650 multilayer switches. Implementation of default gateway redundancy via HSRP (Hot Standby Router Protocol).
- **WAN / Service Provider Segment:** Multi-access network utilizing a Frame Relay cloud (`SW_Cloud`) with DLCI mapping and serial PPP links.
- **External & Edge Segments:** Public network (`PUBLIC` with a Cloud server in `198.51.100.0/26`) and Remote network (`Remote` utilizing NAT translation on an edge router serving `172.25.10.0/24`).

### Project / Lab Catalog
- **[Lab 00] Topology Preparation & Base Addressing (`exc_00_topology_preparation`)**
  Initialization and complete physical/logical cabling of a WAN demonstration topology. Designing and deploying a custom IPv4 addressing scheme (private & public), configuring 802.1Q subinterfaces, gateway DHCP servers, HSRP redundancy, static Frame Relay mapping, and NAT Overload for remote branch access.