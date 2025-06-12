

### **Vergleich: Wi-Fi vs. Zigbee**
| **Merkmal**              | **Wi-Fi (Raspberry Pi)**         | **Zigbee**                          |
|---------------------------|-----------------------------------|--------------------------------------|
| **Hardwarekosten**        | Keine zusätzlichen Kosten        | Zusätzliche Module erforderlich (ca. 10–30 EUR) |
| **Geschwindigkeit**       | Bis zu 150 Mbps                 | Bis zu 250 kbps                     |
| **Reichweite**            | 30–50 m (erweiterbar mit Repeatern) | 10–100 m (erweiterbar durch Mesh)   |
| **Energieverbrauch**      | Höher                           | Sehr niedrig                        |
| **Netzwerkstruktur**      | Infrastruktur (Router-basiert)   | Mesh-Netzwerk                       |
| **Komplexität**           | Einfach (Standard-Wi-Fi-Protokoll) | Höher (Zigbee-Stack erforderlich)   |

Hier ist ein Vergleich zwischen **CAN (Controller Area Network)** und **Zigbee**, zwei sehr unterschiedlichen Kommunikationsprotokollen, die für unterschiedliche Anwendungsbereiche entwickelt wurden:

---

### **Vergleich: CAN vs. Zigbee**

| **Merkmal**                | **CAN (Controller Area Network)**           | **Zigbee**                                |
|-----------------------------|----------------------------------------------|-------------------------------------------|
| **Typ**                    | Kabelgebundenes serielles Protokoll          | Drahtloses Mesh-Netzwerkprotokoll         |
| **Signalprinzip**          | Differenziell (CAN High und CAN Low)         | Funkübertragung (IEEE 802.15.4, 2.4 GHz) |
| **Kommunikationsstruktur** | Multimaster-Bus                             | Mesh-, Stern- oder Baum-Topologie         |
| **Adressierung**           | Nachrichtenbasierte IDs                     | Geräteadressierung (16- oder 64-Bit-Adressen) |
| **Geschwindigkeit**        | Bis zu 1 Mbps (CAN FD: 8 Mbps)              | Bis zu 250 kbps                           |
| **Reichweite**             | Bis zu 1 km bei niedrigen Datenraten        | Typisch 10–100 Meter (erweiterbar durch Mesh) |
| **Fehlersicherheit**       | CRC, Error Frames, automatische Wiederholungen | CRC, aber weniger robust als CAN          |
| **Energieverbrauch**       | Relativ hoch (kabelgebunden, keine Energiesparmodi) | Sehr niedrig (optimiert für batteriebetriebene Geräte) |
| **Netzwerkstruktur**       | Bus mit Multimaster-Fähigkeit               | Mesh-Netzwerk mit Routing-Fähigkeit       |
| **Anwendungsbereich**      | Fahrzeuge, Industrie, IoT                   | Smart Home, IoT, Sensornetzwerke          |
| **Kosten**                 | Höher (CAN-Controller und Transceiver erforderlich) | Niedrig (kostengünstige Funkmodule)       |



7. Secure Shell

Das SSH-Protokoll bietet eine Möglichkeit, über ein unsicheres Netzwerk, zum Beispiel das Internet, eine sichere Verbindung zu einem Gerät herzustellen und Befehle an dieses zu senden. Es verwendet Kryptografie zur Authentifizierung und baut einen verschlüsselten digitalen Tunnel zwischen den Geräten auf, der die Kommunikation vor Abhörversuchen und Manipulationen schützt.

SSH wird häufig für die Fernverwaltung von Servern, Netzwerkgeräten und anderen Systemen verwendet. Es automatisiert verschiedene Aufgaben auf diesen Remote-Systemen, darunter Software-Updates, Backups und Systemüberwachung. Darüber hinaus bietet es Tunneling oder Portweiterleitung, wodurch Datenpakete Netzwerke durchqueren können, auf die sonst kein Zugriff möglich wäre.

Quelle:
https://www.computerweekly.com/de/feature/12-gaengige-Netzwerkprotokolle-und-ihre-Funktionsweise

(siehe dort weiteres zu UDP/IP, TCP/IP, HTTPS, FTP usw.)







### **1.TCP/IP- vs. OSI-Modell**

Das **TCP/IP-Modell** und das **OSI-Modell** sind zwei unterschiedliche Referenzmodelle, die die Struktur und Funktionsweise von Netzwerken beschreiben. Es gibt jedoch Überschneidungen zwischen den beiden Modellen. 

#### **Vergleich von TCP/IP und OSI-Modell**
| **OSI-Modell (7 Schichten)**   | **TCP/IP-Modell (4 Schichten)**         | **Beispiele für Protokolle**            |
|--------------------------------|-----------------------------------------|-----------------------------------------|
| **7. Anwendungsschicht**       | **4. Anwendungsschicht**               | HTTP, FTP, SMTP, DNS                   |
| **6. Darstellungsschicht**     | **(Teil der Anwendungsschicht)**        | SSL/TLS, MIME                          |
| **5. Sitzungsschicht**         | **(Teil der Anwendungsschicht)**        | NetBIOS, RPC                           |
| **4. Transportschicht**        | **3. Transportschicht**                | TCP, UDP                               |
| **3. Vermittlungsschicht**     | **2. Internetschicht**                 | IP, ICMP, ARP                          |
| **2. Sicherungsschicht**       | **1. Netzwerkschicht (Link Layer)**    | Ethernet, Wi-Fi, PPP                   |
| **1. Bitübertragungsschicht**  | **(Teil der Netzwerkschicht)**          | Physische Medien (z. B. Kabel, Funk)   |

#### **Unterschiede**:
- Das **TCP/IP-Modell** hat nur **4 Schichten**, während das **OSI-Modell** 7 Schichten hat.
- Im TCP/IP-Modell werden die **Darstellungs-** und **Sitzungsschicht** des OSI-Modells in die **Anwendungsschicht** integriert.
- Die **Bitübertragungs-** und **Sicherungsschicht** des OSI-Modells werden im TCP/IP-Modell zur **Netzwerkschicht (Link Layer)** zusammengefasst.

---

### **2. Braucht es für jede Anwendung alle Schichten und ein Protokoll pro Schicht?**

Es brauchst nicht immer alle Schichten oder ein Protokoll für jede Schicht. Es hängt von der Anwendung und dem Kommunikationsszenario ab. 

#### **Wann werden alle Schichten benötigt?**
- In den meisten modernen Netzwerken werden **alle Schichten** verwendet, da sie zusammenarbeiten, um die Kommunikation zu ermöglichen.
- Jede Schicht hat eine spezifische Aufgabe:
  - **Anwendungsschicht**: Stellt die Schnittstelle für Anwendungen bereit (z. B. HTTP für Webbrowser).
  - **Transportschicht**: Sorgt für zuverlässige Datenübertragung (z. B. TCP) oder schnelle, unzuverlässige Übertragung (z. B. UDP).
  - **Internetschicht**: Kümmert sich um die Adressierung und das Routing (z. B. IP).
  - **Netzwerkschicht**: Überträgt die Daten physisch über das Medium (z. B. Ethernet, Wi-Fi).

#### **Wann werden nicht alle Schichten benötigt?**
- **Lokal begrenzte Kommunikation**:
  - Wenn zwei Geräte direkt über ein lokales Netzwerk (z. B. Ethernet) kommunizieren, wird die Internetschicht (IP) möglicherweise nicht benötigt.
- **Spezialisierte Protokolle**:
  - Manche Protokolle arbeiten nur auf bestimmten Schichten. Beispiel:
    - **ICMP** (Internet Control Message Protocol) arbeitet nur auf der Internetschicht.
    - **Ethernet** arbeitet nur auf der Netzwerkschicht.

#### **Protokoll pro Schicht?**
- In der Praxis wird oft **ein Protokoll pro Schicht** verwendet, aber es ist nicht zwingend erforderlich. Manche Anwendungen oder Netzwerke verwenden mehrere Protokolle auf einer Schicht oder überspringen Schichten.
  - Beispiel:
    - **HTTP** (Anwendungsschicht) verwendet **TCP** (Transportschicht), das wiederum **IP** (Internetschicht) und **Ethernet** (Netzwerkschicht) nutzt.
    - **VoIP** (Voice over IP) verwendet **RTP** (Anwendungsschicht) über **UDP** (Transportschicht).

---

### **3. Beispiele für Anwendungen und benötigte Schichten**
| **Anwendung**         | **Benötigte Schichten**                     | **Protokolle**                          |
|------------------------|---------------------------------------------|-----------------------------------------|
| **Webbrowser (HTTP)**  | Anwendung, Transport, Internet, Netzwerk   | HTTP, TCP, IP, Ethernet                 |
| **E-Mail (SMTP)**      | Anwendung, Transport, Internet, Netzwerk   | SMTP, TCP, IP, Ethernet                 |
| **VoIP (Telefonie)**   | Anwendung, Transport, Internet, Netzwerk   | RTP, UDP, IP, Ethernet                  |
| **Ping (ICMP)**        | Internet, Netzwerk                         | ICMP, IP, Ethernet                      |
| **Direkte Verbindung** | Netzwerk                                   | Ethernet                                |

---

### **Fazit**
- Das **TCP/IP-Modell** ist nicht einfach die obersten 4 Schichten des OSI-Modells, sondern eine vereinfachte und praxisorientierte Alternative.
- Für die meisten Anwendungen werden **alle Schichten** benötigt, da sie zusammenarbeiten, um die Kommunikation zu ermöglichen.
- Du brauchst jedoch nicht immer ein Protokoll für jede Schicht. Manche Anwendungen oder Szenarien verwenden nur bestimmte Schichten oder Protokolle. Die Wahl der Schichten und Protokolle hängt von der Art der Kommunikation und den Anforderungen der Anwendung ab.


### **Quellen:**

- **RFC-Dokumente**:
  - Das TCP/IP-Modell ist in den **RFC-Dokumenten** (Request for Comments) beschrieben, insbesondere:
    - [RFC 791 (IP)](https://www.rfc-editor.org/rfc/rfc791.html)
    - [RFC 793 (TCP)](https://www.rfc-editor.org/rfc/rfc793.html)
    - [RFC 768 (UDP)](https://www.rfc-editor.org/rfc/rfc768.html)

- **Computer Networking Bücher**:
  - "Computer Networking: Principles, Protocols, and Practice" von Olivier Bonaventure.
  - "Computer Networks" von Andrew S. Tanenbaum.

- **Technische Artikel**:
  - [12 gängige Netzwerkprotokolle und ihre Funktionsweise](https://www.computerweekly.com/de/feature/12-gaengige-Netzwerkprotokolle-und-ihre-Funktionsweise) 

- **Wikipedia**:
  - [OSI-Modell](https://de.wikipedia.org/wiki/OSI-Modell)
  - [TCP/IP-Modell](https://de.wikipedia.org/wiki/TCP/IP-Modell)

---