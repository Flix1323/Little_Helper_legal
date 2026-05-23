# Datenschutzerklärung – Little Helper

**Stand:** Mai 2026  
**Verantwortlicher:** [Dein Name / Unternehmensname], [Adresse] – [E-Mail]

---

## 1. Überblick

Little Helper ist eine iOS/iPadOS/macOS/watchOS-App zur Verfolgung von Gewohnheiten, Stimmung, Wasseraufnahme, Schlaf, Aufgaben und Fokustraining. Alle Daten werden **ausschließlich lokal** auf deinem Gerät gespeichert. Es gibt keine Nutzungsanalyse, kein Tracking, keine Werbung und keine Weitergabe an Dritte.

---

## 2. Welche Daten werden verarbeitet?

### 2.1 Von dir eingegebene Daten (lokal, niemals übertragen)

| Datenkategorie | Beispiele | Zweck |
|---|---|---|
| Name & Benutzername | Profilname | Personalisierung |
| E-Mail-Adresse | Lokales Konto | Anmeldung |
| Persönliche Daten | Geburtsdatum, Geschlecht | Optionale Personalisierung |
| Gewohnheiten & Routinen | Titel, Häufigkeit, Fortschritt | Kernfunktion |
| Stimmungseinträge | Stimmungswert, Notiz, Zeitstempel | Selbstreflexion |
| Glücksmomente | Fotos, Texte | Persönliches Tagebuch |
| Wasseraufnahme | Mengen, Zeitstempel | Gesundheitsverfolgung |
| Schlaf | Schlafdauer, Qualität | Gesundheitsverfolgung |
| Fokussitzungen | Dauer, Thema | Produktivität |
| Aufgaben & Kategorien | Titel, Fälligkeiten | Aufgabenverwaltung |
| Profilbild | Optional hochgeladen | Personalisierung |

### 2.2 Apple Health (HealthKit)

Die App kann auf Wunsch Daten aus Apple Health lesen (Wasser, Schlaf, Schritte). Du gibst diese Berechtigung explizit über das iOS-Berechtigungsdialog. Die Daten werden **nicht** an Server übertragen. Wassereinträge können optional in Health zurückgeschrieben werden.

### 2.3 Ungefährer Standort (Coarse Location)

Der Standort wird einmalig pro Session abgefragt, um den aktuellen Wetterzustand (klar, bewölkt, Regen) für den animierten Garten-Hintergrund zu ermitteln. Es wird ausschließlich eine gerundete Koordinate (1 Dezimalstelle) an den Little Helper Weather Proxy auf Cloudflare übermittelt. Der Proxy gibt keine Standortdaten weiter und speichert sie nicht dauerhaft. Du kannst die Berechtigung jederzeit unter Einstellungen › Datenschutz & Sicherheit › Ortungsdienste entziehen.

### 2.4 KI-Funktionen (Apple Intelligence)

Alle KI-Funktionen (Companion-Antworten, Tagesplanung, Zusammenfassungen) nutzen ausschließlich Apple Intelligence – ein On-Device-Modell von Apple. Es werden **keine Nutzerdaten an externe KI-Server** übertragen. Das Modell läuft vollständig auf deinem Gerät. Für Geräte ohne Apple Intelligence stehen lokale Fallback-Texte bereit.

---

## 3. Datenübertragungen

Die einzige externe Datenübertragung ist der Wetter-Request an den Cloudflare Worker (`littlehelper.sxvdyn64h5.workers.dev`). Dabei wird ausschließlich eine gerundete Koordinate (Breitengrad, Längengrad auf 1 Dezimalstelle) übermittelt. Der Worker gibt keine weiteren Nutzerdaten weiter.

Es gibt **keine Verbindung** zu Analytics-Diensten, Werbenetzwerken oder sozialen Plattformen.

---

## 4. iCloud-Synchronisierung

iCloud-Sync (CloudKit) ist aktuell **nicht aktiviert**. Alle Daten verbleiben lokal auf deinem Gerät. Eine zukünftige Version kann optional iCloud-Sync anbieten – dies wird dann gesondert kommuniziert.

---

## 5. Drittanbieter-SDKs

Die App verwendet **keine Drittanbieter-SDKs**. Es sind ausschließlich Apple-eigene Frameworks im Einsatz (SwiftUI, SwiftData, HealthKit, CoreLocation, AVFoundation, WatchConnectivity u. a.).

---

## 6. Deine Rechte

- **Auskunft:** Du kannst jederzeit nachfragen, welche Daten die App lokal über dich gespeichert hat.
- **Löschung:** Du kannst alle Daten unter Einstellungen › Konto-Verwaltung › Konto löschen vollständig und unwiderruflich entfernen.
- **Daten aus Apple Health:** Einträge, die Little Helper in Apple Health gespeichert hat, kannst du in der Health-App unter Einstellungen › Datenschutz & Sicherheit › Health entfernen.
- **Widerspruch:** Du kannst die Ortungsberechtigung jederzeit entziehen. Die App läuft ohne Standortzugriff weiter – der Garten-Hintergrund zeigt dann einen Standard-Wetterzustand.

---

## 7. Sicherheit

Alle Daten liegen in der SwiftData-Datenbank, die durch die iOS-Geräteverschlüsselung (Secure Enclave) geschützt ist. Passwörter werden nicht im Klartext gespeichert, sondern als CryptoKit-Hash.

---

## 8. Kinder

Little Helper richtet sich nicht an Kinder unter 13 Jahren. Es werden keine Daten von Kindern absichtlich erfasst.

---

## 9. Änderungen dieser Erklärung

Änderungen an dieser Datenschutzerklärung werden in der App kommuniziert. Die aktuell gültige Version ist immer unter [https://littlehelper.app/privacy](https://littlehelper.app/privacy) abrufbar.

---

## 10. Kontakt

Bei Fragen zum Datenschutz:  
**E-Mail:** support@littlehelper.app  
<!-- TODO: Adresse und ggf. Impressum ergänzen (bei EU-Nutzern gesetzlich erforderlich) -->
