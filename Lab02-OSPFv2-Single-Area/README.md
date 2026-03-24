# Lab 02: Routing dynamiczny OSPFv2 (Single-Area)

---

## 🇵🇱 Wersja Polska

### Opis projektu
Laboratorium skupiało się na wdrożeniu protokołu stanu łącza **OSPFv2** w obrębie jednego obszaru (**Area 0**). Głównym celem było zrozumienie działania algorytmu Dijkstry oraz mechanizmów wyboru optymalnej trasy.

### Kluczowe zadania i protokoły
* **Konfiguracja OSPF:** Ustawianie unikalnych Router ID oraz rozgłaszanie sieci w procesie OSPF.
* **Inżynieria ruchu:** Ręczna manipulacja metryką poprzez zmianę przepustowości (`bandwidth`) oraz kosztu interfejsów (`ip ospf cost`).
* **Optymalizacja:** Konfiguracja interfejsów pasywnych (`passive-interface`) w celu zwiększenia bezpieczeństwa i ograniczenia zbędnego ruchu w sieciach lokalnych.
* **Analiza:** Weryfikacja tablic routingu oraz bazy danych LSDB.

**Topologia:**
![Screenshot](./topology.png)

---

## 🇬🇧 English Version 

### Project Description
This lab focused on implementing the **OSPFv2** link-state protocol within a single backbone area (**Area 0**). The primary objective was to understand the Dijkstra algorithm and path selection mechanisms.

### Key Tasks & Protocols
* **OSPF Configuration:** Setting unique Router IDs and advertising networks within the OSPF process.
* **Traffic Engineering:** Manual metric manipulation by adjusting `bandwidth` and `ip ospf cost` parameters.
* **Optimization:** Configuring `passive-interface` to enhance security and reduce unnecessary OSPF overhead in local networks.
* **Diagnostics:** Verification of routing tables and the Link-State Database (LSDB).

**Topology:**
![Screenshot](./topology.png)