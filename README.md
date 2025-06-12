# 🔧 Mein Tech-Stack & Projekte (Portfolio)

## 🚀 Technologien, mit denen ich vor 2025 gearbeitet habe:

- **Microcontroller**: ARM, Raspberry Pi 3B , Arduino Uno, Atmel ATmega328PB
- **FPGA**: Artix-7, Zynq-7000, 
- **Kommunikation**: RS422, RS232, LVDS, special with x-Heep
- **Protokolle**: SpaceWire, AXI, AMBA, UART, SPI, special
- **Containerisierung**: Docker, Docker Compose
- **Entwicklungstools**: GitHUB & GitLab, VS Code, DesignSpark, Malab & SimuLink, Vivado, Quartus Prime, Nios2, EPLAN, Cameo, Confluence
- **Systeme**: OpenMediaVault, Linux, Windows

## 📚 Projekte (Beendet)

| Projekt                                                                             | Technologien & Programme            | Link              |
|-------------------------------------------------------------------------------------|-------------------------------------|-------------------|
| Entwicklung einer Vorstufe für eine portable Audiobox (2 Monate)                        | TDA1524A(IC),  Platine selbst geäzt & DesignSpark(PCB Tool)   | firmenintern |
| Erweiterung eines Position-Simulators für ein Scaninstrument eines Satelliten (4 Monate)| Zynq-7000 SoC(FPGA & ARM) & Xilinx Vivado, PetaLinux, MacroCode  | firmenintern    |   
| Sichtfeldsimulator eines Helikopters (3 Monate)                                         | Simulink & Matlab               | Forschungsintern  |
| Abbildung einer Antennensteuerung für komplexe Bewegungsprofile in Software (3 Monate)  | SoC(FPGA & ARM), FPU & Xilinx/AMD Vivado| firmenintern      |
| FPGA Projekt mit Sensoren und Regelung (5 Monate)                                       | SoC(FPGA & ARM) & Intel Quartus Prime, Nios2, Ubuntu        | Forschungsintern  |
| Fahrrradcomputer als FPGA Project  (2 Monate)                                           | SoC(FPGA & ARM) & Vivado, Ubuntu        | Forschungsintern  |
| Enabling Inference of Transformer Networks (LLM) on a SoC (6 Monate)                    | RISC-V, SoC & x-Heep, Ubuntu, Vivado     | Forschungsintern  |


## 📚 Projekte (Ausstehend)

| Projekt noch in Bearbeitung:                                                            | Technologien                        | Link         |
|-----------------------------------------------------------------------------------------|-------------------------------------|--------------|
| Hausautomation mit ESP32 & MQTT                                                         | ESP32, MQTT, Node-RED               | [Repo](...)  |
| NAS mit OpenMediaVault & Plex                                                           | Raspberry Pi, OMV, Plex, Docker     | [Repo](...)  |
| CAN↔RS485 Brücke                                                                        | CAN, RS485, STM32                   | [Repo](...)  |
| lokaler AI Butler zur Hausauotmation und Dateiverwaltung                                | Raspberry Pi,                  | [Repo](...)  |


Ich habe umfassende praktische Erfahrung in der Entwicklung und Implementierung von Embedded-Systemen. Dabei habe ich mich intensiv mit den Prinzipien der **Direct Memory Access (DMA)** und der **Hardware Abstraction Layer (HAL)** auseinandergesetzt, um die Effizienz und Modularität von Firmware zu steigern. Dabei konnte ich sowohl die Hardware- als auch die Softwareebene optimieren, um zuverlässige und leistungsfähige Lösungen zu entwickeln. Meine Arbeit umfasst die Integration dieser Technologien in Echtzeitsysteme sowie die Entwicklung effizienter Lösungen für Mikrocontroller und FPGA.

Ich habe mit einer Vielzahl von Kommunikationsprotokollen, darunter **UART**, **SPI**, **RS422**, **RS232** und **SpaceWire**, gearbeitet und diese erfolgreich in komplexe Systeme integriert. 

Hier eine genaue Übersicht, welche Konzepte bereits praktisch von mir umgesetzt wurde und welche noch ausstehen:

# ✅ Embedded Developer To-Do Liste

## 🛠️ Hardware-nahe Programmierung
- <span style="color:green;">✔️</span> **Register-Level-Programmierung**: Direkte Manipulation von Hardware-Registern (z. B. GPIO, Timer, ADC).
- [ ] **Interrupts**: Implementierung von Interrupt-Service-Routinen (ISR).
- <span style="color:green;">✔️</span> **Direct Memory Access (DMA)**: Effiziente Datenübertragung ohne CPU-Belastung.

---

## 🧩 Software-Abstraktion
- <span style="color:green;">✔️</span> **Hardware Abstraction Layer (HAL)**: Nutzung von HAL-Bibliotheken (z. B. STM32 HAL, CMSIS).
- <span style="color:green;">✔️</span> **Treiberentwicklung**: Schreiben von Treibern für Peripheriegeräte (Sensoren, Displays, Kommunikationsmodule).

---

## ⏱️ Echtzeitprogrammierung
- [~] **Real-Time Operating Systems (RTOS)**: Verständnis von Tasks, Semaphoren, Mutexes und Queues (z. B. FreeRTOS, Zephyr).
- <span style="color:green;">✔️</span> **Task-Scheduling**: Implementierung von kooperativen oder präemptiven Scheduler-Mechanismen.

---

## 🔗 Kommunikationsprotokolle
- [~] **Serielle Protokolle**: UART, SPI, I2C – Konfiguration und Nutzung.
- [ ] **Netzwerkprotokolle**: CAN, Ethernet, MQTT, Modbus – Implementierung und Optimierung.
- [ ] **Drahtlose Protokolle**: Zigbee, LoRa, Bluetooth, Wi-Fi – Integration und Konfiguration.

---

## 💾 Speicherverwaltung
- [~] **Flash-Speicher**: Schreiben, Lesen und Löschen von Daten im Flash-Speicher.
- <span style="color:green;">✔️</span> **RAM-Optimierung**: Effiziente Nutzung des begrenzten RAM-Speichers.

---

## 🐞 Debugging und Fehlerbehandlung
- <span style="color:green;">✔️</span> **Debugging-Tools**: Nutzung von JTAG, GDB (oder ST-Link, SWD).
- [ ] **Fehlerbehandlung**: Implementierung von Watchdog-Timern und Fail-Safe-Mechanismen.
- <span style="color:green;">✔️</span> **random number generators** (RNGs) for unit testing 
- [~] **real time clock** (rtc) use or different concepts 
---

## 🔋 Energiemanagement
- [~] **Low-Power-Design**: Nutzung von Sleep- und Deep-Sleep-Modi für energieeffiziente Systeme.

---

## 🔒 Sicherheitskonzepte
- [ ] **Secure Boot**: Authentifizierung und Integritätsprüfung der Firmware.
- [~] **Verschlüsselung**: Nutzung von kryptografischen Algorithmen für sichere Kommunikation und Datenspeicherung.

---

## 🖥️ Embedded Software-Design
- :white_check_mark: **State Machines**: Implementierung von Zustandsautomaten für komplexe Abläufe.
- :white_check_mark: **Modularisierung**: Schreiben von modularem und wiederverwendbarem Code.
- :white_check_mark: **Testbarkeit**: Unit-Tests und Integrationstests für Embedded-Systeme.

---

## 📊 Weitere wichtige Konzepte
- :white_check_mark: **Signalverarbeitung**: Grundlagen der digitalen Signalverarbeitung (DSP).
- :white_check_mark: **Zeitmanagement**: Nutzung von Timern und Zeitgebern für zeitkritische Anwendungen.
- [~] **Bootloader**: Entwicklung und Nutzung von Bootloadern für Firmware-Updates und Sicherheitsfunktionen.

---



# ✅ Moderne C-Programmierung To-Do Liste

## 🛠️ Prozedurale Programmierung
- :white_check_mark: **Modularisierung**: Zerlege Code in kleine, wiederverwendbare Funktionen und Module.
- :white_check_mark: **Klares Funktionsdesign**: Schreibe Funktionen mit klar definierten Eingaben und Ausgaben.
- :white_check_mark: **Vermeidung globaler Variablen**: Nutze lokale Variablen und Parameter.

---

## 💾 Speicherverwaltung
- :white_check_mark: **Manuelle Speicherverwaltung**: Verstehe `malloc`, `calloc`, `realloc` und `free`.
- :white_check_mark: **Stack vs. Heap**: Nutze den Stack für lokale Variablen und den Heap für dynamische Speicherzuweisungen.
- [~] **Speicherlecks vermeiden**: Implementiere klare Ownership-Regeln.

---

## 📐 Effiziente Datenstrukturen
- :white_check_mark: **Arrays und Pointer**: Verstehe Pointer-Arithmetik und dynamische Arrays.
- :white_check_mark: **Strukturen (`struct`)**: Nutze `struct`, um komplexe Datenstrukturen zu erstellen.

---

## 🐞 Fehlerbehandlung
- :white_check_mark: **Rückgabewerte prüfen**: Überprüfe Rückgabewerte von Funktionen (z. B. `NULL` oder negative Werte).
- [~] **Defensive Programmierung**: Implementiere Sicherheitsprüfungen (z. B. Null-Pointer oder Array-Grenzen).

---

## 🔗 Hardware-nahe Programmierung
- :white_check_mark: **Register-Level-Programmierung**: Arbeite direkt mit Hardware-Registern.
- :white_check_mark: **Bitmanipulation**: Verstehe Bitmasken, Bit-Shift-Operationen und Flags.

---

## ⏱️ Effiziente Algorithmen
- [~] **Optimierung**: Schreibe effizienten Code, der Speicher und CPU-Zyklen spart.
- :white_check_mark: **Inline-Funktionen**: Nutze `inline`, um kleine Funktionen direkt im Code zu platzieren.

---

## 🐞 Debugging und Testing
- :white_check_mark: **Debugging-Tools**: Nutze Tools wie `gdb`, Valgrind oder andere Debugger.
- :white_check_mark: **Unit-Tests**: Schreibe Tests für einzelne Funktionen.

---

## 🌍 Portabilität
- :white_check_mark: **Plattformunabhängiger Code**: Nutze `<stdint.h>` für portable Datentypen.
- :white_check_mark: **Makros und Präprozessor**: Nutze `#define` und `#ifdef` für plattformabhängige Anpassungen.

---

## 🔒 Sicherheitskonzepte
- :white_check_mark: **Buffer Overflow vermeiden**: Vermeide unsichere Funktionen wie `gets` und nutze `fgets`.
- :white_check_mark: **Konstante Zeiger und Daten**: Nutze `const`, um unbeabsichtigte Änderungen zu verhindern.

---


# ✅ Embedded-C++-Programmierung To-Do Liste

## 🛠️ Objektorientierte Programmierung
- :white_check_mark: **Klassen und Objekte**: Verstehe die Grundlagen von Klassen und Objekten.
- :white_check_mark: **Vererbung**: Implementiere Vererbung für wiederverwendbaren Code.
- :white_check_mark: **Polymorphismus**: Nutze virtuelle Funktionen für flexible Designs.

---

## 🔧 Speicherverwaltung
- [ ] **Smart Pointer**: Verstehe `std::unique_ptr` und `std::shared_ptr` für sichere Speicherverwaltung.
- :white_check_mark: **RAII (Resource Acquisition Is Initialization)**: Nutze Konstruktoren und Destruktoren für Ressourcenmanagement.
- :white_check_mark: **Manuelle Speicherverwaltung vermeiden**: Reduziere die Nutzung von `new` und `delete`.

---

## ⏱️ Echtzeitprogrammierung
- [ ] **Threads und Synchronisation**: Nutze `std::thread`, Mutexes und Condition Variables.
- [ ] **RTOS-Integration**: Implementiere C++-Code in Echtzeitbetriebssystemen (z. B. FreeRTOS).

---

## 🔗 Kommunikationsprotokolle
- :white_check_mark: **Abstraktion durch Klassen**: Implementiere Protokolle wie UART, SPI, I2C als Klassen.
- [ ] **Callback-Mechanismen**: Nutze Funktionszeiger oder `std::function` für flexible Designs.

---

## 🐞 Debugging und Testing
- [ ] **Unit-Tests mit Google Test**: Schreibe Tests für Klassen und Funktionen.
- [ ] **Debugging mit Tools**: Nutze Debugger wie GDB oder IDEs mit C++-Support.

---

## 🔋 Energiemanagement
- [~] **Low-Power-Design**: Implementiere Sleep-Modi und energieeffiziente Algorithmen.
- :white_check_mark: **Hardware-Abstraktion**: Nutze C++-Klassen für Low-Power-Peripherie.

---

## 🔒 Sicherheitskonzepte
- [ ] **Secure Boot**: Implementiere Sicherheitsmechanismen für Firmware-Authentifizierung.
- [ ] **Verschlüsselung**: Nutze kryptografische Bibliotheken wie OpenSSL oder mbedTLS.

---

## 📊 Weitere wichtige Konzepte
- :white_check_mark: **State Machines**: Implementiere Zustandsautomaten mit Klassen.
- [~] **Template-Programmierung**: Nutze Templates für generischen und wiederverwendbaren Code.
- :white_check_mark: **Design Patterns**: Verstehe Muster wie Singleton, Factory und Observer.
