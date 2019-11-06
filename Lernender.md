# Serviceauftrag RasPi-Werkstatt: NAS Pi - Lernender
```
+--Dokumentation Lernender----------------+
! Autoren: Severin Sieber | Roman Signer  !
+-----------------------------------------+
! Version: 1.3                            !
+-----------------------------------------+
```
## Inhaltsverzeichnis
- [Serviceauftrag RasPi-Werkstatt: NAS Pi - Lernender](#serviceauftrag-raspi-werkstatt-nas-pi---lernender)
  - [Inhaltsverzeichnis](#inhaltsverzeichnis)
  - [01 Einführung](#01-einf%c3%bchrung)
    - [Kompakt & Portabel](#kompakt--portabel)
    - [Daten speichern und synchronisieren](#daten-speichern-und-synchronisieren)
    - [Verbindungsprobleme und andere mögliche Stolpersteine](#verbindungsprobleme-und-andere-mögliche-stolpersteine)
  - [02 Materialliste](#02-materialliste)
    - [02.1 Hardware](#021-hardware)
    - [02.2 Software](#022-software)
  - [03 Aufgabenstellung](#03-installationsanleitung)
  - [04 Qualitätskontrolle](#04-qualit%c3%a4tskontrolle)
  - [05 Error-Handling](#05-error-handling)

## 01 Einführung
Bestimmt wolltest du schon einmal von verschiedenen Geräten aus, in deinem privaten Netzwerk, auf deine persönlichen Dateien, Videos und Musik zugreifen aber konntest dir bisher kein teures NAS leisten. Mit unserem Serviceauftrag wollen wir dir dabei helfen, deinen eigenen und erst noch kostengünstigen NAS-Server zu bauen.  

### Kompakt & Portabel
Für die meisten Funktionen, welche man von einem NAS erwartet, reicht ein Raspberry Pi 2, 3, oder noch besser ein Raspberry Pi 4 aus. Der Raspi bietet zwar im Vergleich zu einer NAS-Box, nie dieselbe Prozessorleistung und Übertragungsrate, doch dafür kann er mit seiner Kompaktheit, Portabilität sowie den geringen Anschaffungs- und Energiekosten punkten.  

### Daten speichern und synchronisieren
Um den eigenen NAS-Server zu betreiben, wird neben einem Raspberry Pi nur noch mindestens ein USB-Stick oder eine USB-Festplatte und eine NAS-Server-Software benötigt. Im Internet finden sich einige kostenlose Lösungen, wir möchten jedoch OpenMediaVault empfehlen. OpenMediaVault ist eine Open Source NAS-Server-Software und bietet Funktionen zum Speichern und Verwalten von Dateien an. Für den Fernzugriff auf das NAS unterstützt sie FTP, TFTP, SMB, NFS und SNMP; somit kommt man von praktisch jedem Gerät aus an die eigenen Daten.  
Zur Datensicherung bietet OpenMediaVault die Synchronisation mit Rsync an. Damit kann festgelegt werden, welche Verzeichnisse gesichert und welche nicht gesichert werden sollen.  

### Verbindungsprobleme und andere mögliche Stolpersteine  
Wie es beim realisieren technischer Lösungen leider oft so ist, funktioniert nicht immer alles reibungslos. Die Installation und Konfiguration vom eigenen NAS Pi mit OpenMediaVault ist zwar sehr unkompliziert und in der Regel schnell gemacht, doch auch hier können einige Stolpersteine dafür sorgen, dass einige Lektionen für die Suche nach Problemlösungen geopfert werden müssen. Um dies zu verhindern, zählen wir die Probleme mit möglichen Lösungsansätzen auf, die uns bekannt sind.  

| Problem | Beschrieb | Lösungsansatz |
|:---------|:---------------|:--------|
| Raspberry Pi offline | Obwohl der Raspi mit eingesteckter microSD-Karte läuft und im LAN auftauchen sollte, <br> erscheint dieser nicht in den Suchergebnissen des IP-Scanners. | - Monitor an Raspi anschliessen, Status prüfen <br> - Client und Raspi im selben Netz? <br> - Raspi austauschen <br> - microSD-Karte richtig geflasht? |
| Verbindungsprobleme | Der Raspi läuft, aber es kann keine Verbindung zum OpenMediaVault Webinterface <br> hergestellt werden | - Login via Raspi CMC -> *mount -a* <br> - Anderen Browser verwenden |

## 02 Materialliste
Für den eigenen NAS-Server mit OpenMediaVault wird nur wenig Hard- und Softwarte benötigt:  

### 02.1 Hardware
| Material | Funktionalität |
|:---------|:---------------|
| Raspberry Pi 2 / Raspberry Pi 3 / Raspberry Pi 4 | Einplatinencomputer – Funktion als NAS-Server |
| microSD-Karte	| Speicherkarte auf der sich das OS-Image befindet |
| microSD-Kartenleser	| Zum Schreiben des Images auf die microSD-Karte |
| USB-Stick / USB-Festplatte |	Für die Dateiablage |
| Gerät für Verbindungsaufbau zum Raspi	| Am besten eignet sich hierfür ein Notebook |
| evt. Tastatur | Für den direkten Anschluss ans Raspi falls notwendig |
| evt. Monitor | Ebenfalls für den direkten Anschluss ans Raspi falls notwendig |

### 02.2 Software
| Name |	Funktionalität |	Mindestanforderungen |
|:-----|:----------------|:----------------------|
| OpenMediaVault	| Open Source NAS-Server-Software |	CPU: 500MHz Pentium 3 <br> RAM: 128MB <br> Speicherplatz: 2GB |
| Win32 Disk Imager (Windows) <br> ApplePi-Baker v2 (macOS) | Software zum beschreiben (flashen) der microSD-Karte | Windows / Mac Client |
| Angry IP Scanner	| Software zur Aufspürung des Raspberry Pis |	Windows / Mac Client |
| Browser (Chrome, Firefox, Edge, etc.) |	Zugriff auf das OpenMediaVault Webinterface	| Windows / Mac Client |


## 03 Aufgabenstellung
### 03.1 Bewertungsraster  
| Was? | Soll | Punkte | Notiz |
|:---------|:---------------|:-------|:---------|
| Freigebene Ordner | Freigegebene Ordner können aufgerufen und verwendet werden. | 4 |  |
| Uhrzeit | Die Zeit des Nas-Pi ist der lokalen Urzeit angepasst. | 1 |  |
| Administrator Passwort | Das Passwort des Administrators für das WebGUI wurde gewechselt. Zusatzpunkte wenn das Login zusätzlich geschützt wird. | 1-3 |  |
| Dienste funktionieren | Einer oder mehrere passende Dienste wurden eigerichtet. (Verschiedene Arten von File Sharing) | 1-4 |  |
| Benutzer | Es gibt unterschiedliche Benutzer mit Login. | 2 |  |
| Gruppen | Gruppen sind vorhanden und User sind den entsprechenden Gruppen zugewiesen. | 2 |  | 
| Berechtigungen | Für die verschiedenen Gruppen wurden unterschiedliche Berechtigungen vergeben. Diese haben auch einen Einfluss auf die Zugriffsrechte. | 1 |  |
| RAID | Ein beliebiges RAID ist in Verwendung. | 2 |  |
| Plugins eingerichtet | Mindestens eine für den Service passende Erweiterung ist eingerichtet. | 0-6 |  |
| Live-Demo | Der Dienst kann dem Lehrer Live vorgeführt und erklärt werden. | 2 |  |



## 04 Qualitätskontrolle


## 05 Error-Handling