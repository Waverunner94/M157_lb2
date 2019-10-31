# Serviceauftrag RasPi-Werkstatt: NAS Pi - Lernender
```
+--Dokumentation--------------------------+
! Autoren: Severin Sieber | Roman Signer  !
+-----------------------------------------+
! Version: 1.0                            !
+-----------------------------------------+
```
## Inhaltsverzeichnis
- [Serviceauftrag RasPi-Werkstatt: NAS Pi - Lernender](#serviceauftrag-raspi-werkstatt-nas-pi---lernender)
  - [Inhaltsverzeichnis](#inhaltsverzeichnis)
  - [01 Einführung](#01-einf%c3%bchrung)
    - [Kompakt & Portabel](#kompakt--portabel)
    - [Daten speichern und synchronisieren](#daten-speichern-und-synchronisieren)
  - [02 Voraussetzungen](#02-voraussetzungen)
    - [02.1 Hardware](#021-hardware)
    - [02.2 Software](#022-software)
  - [03 Installationsanleitung](#03-installationsanleitung)
  - [04 Testing](#04-testing)
  - [05 Übergabe an den Betrieb](#05-%c3%9cbergabe-an-den-betrieb)
  - [06 Quellen](#06-quellen)

## 01 Einführung
Bestimmt wolltest du schon einmal von verschiedenen Geräten aus, in deinem privaten Netzwerk, auf deine persönlichen Dateien, Videos und Musik zugreifen aber konntest dir bisher kein teures NAS leisten. Mit unserem Serviceauftrag wollen wir dir dabei helfen, deinen eigenen und erst noch kostengünstigen NAS-Server zu bauen.  

### Kompakt & Portabel
Für die meisten Funktionen, welche man von einem NAS erwartet, reicht ein Raspberry Pi 2, 3, oder noch besser ein Raspberry Pi 4 aus. Der Raspi bietet zwar im Vergleich zu einer NAS-Box, nie dieselbe Prozessorleistung und Übertragungsrate, doch dafür kann er mit seiner Kompaktheit, Portabilität sowie den geringen Anschaffungs- und Energiekosten punkten.  

### Daten speichern und synchronisieren
Für den Betrieb des eigenen NAS-Servers wird neben einem Raspberry Pi nur noch mindestens ein USB-Stick oder eine USB-Festplatte und eine NAS-Server-Software benötigt. Im Internet finden sich einige kostenlose Lösungen, wir möchten jedoch OpenMediaVault empfehlen. OpenMediaVault ist eine Open Source NAS-Server-Software und bietet Funktionen zum Speichern und Verwalten von Dateien an. Für den Fernzugriff auf das NAS unterstützt sie FTP, TFTP, SMB, NFS und SNMP; somit kommt man von praktisch jedem Gerät aus an die eigenen Daten.  
Zur Datensicherung bietet OpenMediaVault die Synchronisation mit Rsync an. Damit kann festgelegt werden, welche Verzeichnisse gesichert und welche nicht gesichert werden sollen.  

## 02 Voraussetzungen


### 02.1 Hardware
| Material | Funktionalität |
|:---------|:---------------|
| Raspberry Pi 2 / Raspberry Pi 3 / Raspberry Pi 4 | Einplatinencomputer – Funktion als NAS-Server |
| microSD-Karte	| Speicherkarte auf der sich das OS-Image befindet |
| microSD-Kartenleser	| Zum Schreiben des Images auf die microSD-Karte |
| USB-Stick / USB-Festplatte |	Zur Dateiablage
| Gerät für Verbindungsaufbau zum Raspi	| Am besten eignet sich hierfür ein Notebook |

### 02.2 Software
| Name |	Funktionalität |	Mindestanforderungen |
|:-----|:----------------|:----------------------|
| OpenMediaVault<sub>[1](#1)</sub>	| Open Source NAS-Server-Software |	CPU: 500MHz Pentium 3 <br> RAM: 128MB <br> Speicherplatz: 2GB |
| Win32 Disk Imager (Windows)<sub>[2](#2)</sub> <br> ApplePi-Baker v2 (macOS)<sub>[3](#3)</sub> | Software zum beschreiben (flashen) der microSD-Karte | Windows / Mac Client |
| Angry IP Scanner<sub>[4](#4)</sub>	| Software zur Aufspürung des Raspberry Pis |	Windows / Mac Client |
| Browser (Chrome, Firefox, Edge, etc.) |	Zugriff auf das OpenMediaVault Webinterface	| Windows / Mac Client |


## 03 Installationsanleitung


## 04 Testing


## 05 Übergabe an den Betrieb


## 06 Quellen
*<a name="1">1</a>* 
*<a name="2">2</a>*  
*<a name="3">3</a>*	 
*<a name="4">4</a>*	