# Serviceauftrag RasPi-Werkstatt: NAS Pi - Lehrer
```
+--Dokumentation--------------------------+
! Autoren: Severin Sieber | Roman Signer  !
+-----------------------------------------+
! Version: 1.0                            !
+-----------------------------------------+
```
## Inhaltsverzeichnis
- [Serviceauftrag RasPi-Werkstatt: NAS Pi - Lehrer](#serviceauftrag-raspi-werkstatt-nas-pi---lehrer)
  - [Inhaltsverzeichnis](#inhaltsverzeichnis)
  - [01 Servicebeschrieb](#01-servicebeschrieb)
    - [Funktionen](#funktionen)
  - [02 Voraussetzungen](#02-voraussetzungen)
    - [02.1 Hardware](#021-hardware)
    - [02.2 Software](#022-software)
  - [03 Installationsanleitung](#03-installationsanleitung)
  - [04 Testing](#04-testing)
  - [05 Übergabe an den Betrieb](#05-%c3%9cbergabe-an-den-betrieb)
  - [06 Quellen](#06-quellen)

## 01 Servicebeschrieb
Mithilfe unseres Serviceauftrags haben die Lernenden die Möglichkeit ein eigenes kompaktes und portables NAS auf einem Raspberry Pi aufzusetzen. Der Auftrag ist vor allem an Anfänger gerichtet und bietet einen soliden Einstieg in die zentrale Dateispeicherung im privaten Bereich.  

### Funktionen
-	Speichern und Verwalten von Dateien
-	Fernzugriff über FTP, TFTP, SMB, NFS und SNMP
-	Datensicherung mit Rsync: welche Verzeichnisse werden gesichert, welche nicht
-	Plug-ins: Virenscanner (?)  

## 02 Voraussetzungen
Die von uns gewählte Variante für den eigenen NAS-Server ist unkompliziert, kostengünstig und setzt wenig voraus.  

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
*<a name="1">1</a>* https://www.openmediavault.org/  
*<a name="2">2</a>* https://sourceforge.net/projects/win32diskimager/files/latest/download  
*<a name="3">3</a>*	https://www.tweaking4all.com/hardware/raspberry-pi/applepi-baker-v2/#InstallingApplePiBaker  
*<a name="4">*</a>*	https://angryip.org/download/
