# Neighborhood Electronics & Tinkering Club: Deployment Plan
## A Blueprint for Local Hardware Hacking, Upcycling, and Open-Source Tech

This document serves as the complete implementation plan for establishing a neighborhood **Electronics & Tinkering Club** operating within the MNeighbor Alliance (MNA) framework. 

---

## 🎯 Club Mission
To build a collaborative, neighbor-to-neighbor ecosystem for hardware developers, makers, and hobbyists. By sharing tools, components, and knowledge, we aim to learn electronics, upcycle e-waste, and develop free, open-source alternatives to commercial home automation, security, and communication products.

---

## 🔬 Core Focus Pillars

The club organizes its projects around four major areas of interest:

### 1. Decentralized Communications (LoRa Meshnet)
Building an off-grid communications mesh network using low-power LoRa (Long Range) radios and the open-source **Meshtastic** protocol.
*   **Modem Preset**: Custom `Medium-Fast` preset (US 915 MHz ISM band) to balance signal speed and neighborhood range.
*   **Hardware Tiers**:
    *   *Pocket Node*: LilyGO T-Echo, Heltec V3, or Heltec V4 (with cases) for portable messaging via Bluetooth.
    *   *Home Node*: Heltec V3, Heltec V4, or LilyGO T-Beam plugged near windows for constant local coverage.
    *   *Roof Repeater*: Solar-powered RAK Wireless WisBlock mounted in a weatherproof box at high elevations to bridge adjacent block Links.
*   **Channel Configurations**: Shared `MediumFast` primary channel and custom encrypted `MNA-Mesh` secondary channel.

### 2. DIY Home Automation & Security
Creating low-cost, privacy-respecting alternatives to commercial subscription-based home security cameras, doorbells, and sensors using microcontrollers.
*   **Core Systems**: Raspberry Pi running **Home Assistant** for central coordination, paired with **ESPHome**, **WLED**, or **Tasmota** firmware for sensor nodes.
*   **Active Projects**:
    *   *DIY Smart Doorbells*: ESP32-CAM nodes running custom firmware to send instant notifications and image snapshots to local servers.
    *   *Environmental Sensors*: Low-cost ESP32 nodes checking temperature, humidity, and motion across the home.

### 3. Hardware Upcycling & Salvage
Reducing electronic waste by repurposing old hardware and screens rather than buying new electronics.
*   **Active Projects**:
    *   *Monitor Wall Calendars*: Turning decommissioned laptop LCD screens (re-wired with low-cost controller boards) into smart, low-power wall calendars powered by Raspberry Pis.
    *   *Component Harvesting*: Reclaiming batteries, switches, wires, and power supplies from broken appliances.

### 4. Digital Fabrication & Making
Manufacturing custom brackets, physical enclosures, and tactile community items.
*   **Active Projects**:
    *   *3D Printing*: Designing and printing custom weather-resistant enclosures for outdoor LoRa repeaters, ESP32 sensor housings, and brackets.
    *   *Button-Making*: Designing and pressing physical pins and badges for community messaging, local events, or neighborhood campaigns.

---

## 🛠️ The Shared Community Inventory (The "Makers' Bin")

To lower the barrier of entry for neighbors who want to tinker but lack tools or materials, the club coordinates a shared resource model:

```
[Tool Library] + [Shared Parts Bin] ➔ Zero-Cost Entry for Neighbors
```

### 1. The Tool Library
Members pool high-cost tools that can be borrowed on-demand:
*   Soldering stations (with ventilation fans).
*   Multimeters, logic analyzers, and oscilloscopes.
*   3D printers (PLA/PETG filaments).
*   Heavy-duty button-making press machines.

### 2. The Parts Bin
A community box of low-cost, common components maintained by donation:
*   ESP32 and ESP8266 development boards.
*   Hookup wire, breadboards, headers, and solder.
*   Basic sensors (PIR motion, DHT22 temperature, photoresistors).
*   Spare resistors, capacitors, LEDs, and tactile switches.

---

## 📡 Phase 1: Digital Basecamp & Recruiting

1.  **Digital Basecamp Integration**: The club utilizes the existing neighborhood **Signal Group** and community **Discord Server** for real-time code sharing, troubleshooting, 3D model distribution, and setup help.
2.  **Porch Outreach**: Customize the [Club Interest Flyer Template](file:///c:/Users/donno/source/mneighbor-alliance/templates/CLUB_INTEREST_FLYER.md) listing the Signal/Discord channels and detail the shared tools available.
3.  **Active Routing**: Work with the block **Router** to distribute the flyers locally and forward them to the **Mesh Council** to reach adjacent block Links, finding hidden tinkerers across the neighborhood.

---

## 🎪 Phase 2: Monthly Build Nights & Field Days

*   **Monthly Build Nights**: Held in public library study rooms or member garages. Focus on group assembly (e.g., configuring Home Assistant, soldering sensor nodes, or printing node enclosures).
*   **Neighborhood Field Days**: Hosted within a permitted MNA Link street closure.
    *   *Mesh Radio Range Testing*: Riding bikes to the limits of the mesh to map signal strength.
    *   *DIY Security Demos*: Setting up temporary outdoor doorbell/camera nodes to test trigger latency.
    *   *Button Making Station*: Setting up a folding table for kids and neighbors to design and press custom buttons.

---

## 🛡️ Operating Rules, Safety, & Legal Guardrails

> [!WARNING]
> **Safety and Compliance Mandates**:
> *   **High-Voltage Safety**: Club projects are strictly limited to low-voltage DC electronics (under 24V). Tinkering with 120V AC mains electricity is prohibited at club workshops.
> *   **Lithium Battery Safety**: Any project involving LiPo or 18650 lithium cells must use certified battery management boards (BMS) with overcharge/discharge protection to prevent fire hazards.
> *   **FCC Compliance**: Mesh radio transmitters must comply with low-power license-free ISM regulations. Unauthorized modifications to transmitter power outputs are prohibited.
>
> **MNA Fiduciary Boundary & Non-Endorsement**:
> This blueprint is a peer-to-peer template. MNeighbor Alliance does not sponsor, endorse, support, or assume liability for the activities of the club, home-built security/automation setups, physical installations, or any electrical/fire hazards. Organizers and participants are solely responsible for ensuring complete compliance with FCC rules, municipal electrical codes, private property permissions, and local laws.
