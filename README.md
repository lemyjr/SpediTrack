# SpediTrack 🚚📍

**SpediTrack** ist eine moderne, modulare Speditionsplattform für virtuelle Logistikunternehmen. Sie kombiniert eine webbasierte Benutzerverwaltung mit automatischer Fahrtenerkennung aus **Euro Truck Simulator 2 (ETS2)** und **American Truck Simulator (ATS)** via Telemetrie-Daten. Die Fahrten werden in Echtzeit an das Web-Backend übermittelt und dort auf einer Karte angezeigt.

---

## 🧩 Features

### 🌐 Webplattform
- Benutzerverwaltung mit Rollen (Admin, Disponent, Fahrer)
- Verwaltung von Fahrern, LKWs und Fahrten
- Admin-Panel mit Funktionen zur Passwortvergabe, Mailverifizierung und Rollenverwaltung
- API mit API-Keys für externe Tools oder Apps
- Fahrtenliste mit Filter- und Bearbeitungsfunktion für Disponenten
- Kartenintegration zur Anzeige von Positionen (z. B. Leaflet oder Mapbox)

### 🖥️ C++-Telemetrie-Client (in Entwicklung)
- Liest ETS2/ATS-Telemetriedaten live aus
- Erkennung von Beginn, Ende und Ziel einer Fahrt
- Automatische Übergabe der Fahrt an die Webplattform
- Offline-Pufferung bei Verbindungsverlust
- Unterstützung für modifizierte Karten (z. B. Promods, etc.)

---

## 🛠️ Technologien

- **Backend:** PHP (ohne Composer), MySQL/MariaDB
- **Frontend:** HTML, JavaScript, Bootstrap
- **API:** RESTful unter `/api/v1/`, Authentifizierung über API-Key
- **Telemetrie-Client:** C++ mit Zugriff auf `scs-sdk` oder eigene ETS2/ATS-Telemetrieimplementierung

---

## 🚦 Rollen & Berechtigungen

| Rolle       | Beschreibung                                      |
|-------------|---------------------------------------------------|
| **Admin**   | Vollzugriff auf System und Benutzerverwaltung     |
| **Disponent** | Verwaltung von LKWs und Zuweisung von Fahrten    |
| **Nutzer**  | Reine Nutzung der Plattform (Fahrer)              |

---

## 📦 API

Die API ist erreichbar unter:
`/api/v1/`
Jeder Benutzer erhält automatisch bei Registrierung einen **API-Key**. Dieser kann über das Dashboard angezeigt oder erneuert werden.

---

## 🔐 Sicherheit

- Passwörter werden sicher gehasht
- Rollen- und Rechteverwaltung für jede Seite
- API-Zugriff nur mit gültigem Key
- E-Mail-Verifizierung bei der Registrierung


## 📍 Live-Tracking (in Vorbereitung)

Fahrzeuge werden auf einer Karte angezeigt, sobald die Fahrt beginnt. Es ist geplant, die aktuellen GPS-Daten live zu übertragen und anzuzeigen.

---

## 🧪 Roadmap

- [x] Webplattform Grundstruktur
- [x] Rollen- & Rechteverwaltung
- [x] API mit API-Key-System
- [ ] C++ Telemetrie-Client
- [ ] Automatische Fahrtenerkennung
- [ ] Echtzeitkartenansicht

---

## 🤝 Lizenz

**SpediTrack** ist ein privates Projekt in Entwicklung. Eine Open-Source-Freigabe ist derzeit **nicht** geplant.

---

## 💬 Kontakt

Bei Fragen oder Interesse an einer Zusammenarbeit:
folgt

---

**SpediTrack – Deine virtuelle Spedition auf der Überholspur.**
