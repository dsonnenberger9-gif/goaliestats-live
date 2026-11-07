# GoalieStats Live – öffentliche Beta

Eine statische, installierbare Web-App (PWA). Kein Konto und kein Server für persönliche Spielstatistiken erforderlich.

## Veröffentlichen

1. Ein Konto bei einem geeigneten Hosting-Anbieter anlegen (z. B. Cloudflare Pages; Konditionen prüfen).
2. Den **Inhalt** dieses Ordners (nicht den übergeordneten Ordner) als statische Website hochladen.
3. Nach Veröffentlichung die HTTPS-Adresse auf dem iPhone in **Safari** öffnen.
4. Teilen → Zum Home-Bildschirm. Die App einmal online öffnen, anschließend im Flugmodus testen.
5. Ein Testspiel eingeben, als JSON sichern und Import prüfen, bevor echte Spieldaten erfasst werden.

**Nicht** die HTML-Datei per AirDrop in der iOS-Dateivorschau starten: Dort ist JavaScript nicht zuverlässig verfügbar. Die Offline-Funktion benötigt HTTPS und den Service Worker.

## Funktionsumfang

- Spielstand mit editierbaren Teamnamen
- Schuss gehalten, Gegentor, Tor eigene Mannschaft, Rückgängig
- Zwei Torhüter, Tor leer, Wechsel nach eingegebener Spielminute
- Fangquote je Goalie, Drittel, Rebound, Breakaway; GAA auf 60 Minuten normiert
- Spielarchiv, CSV-Export und JSON-Backup/-Import
- Speicherung lokal im Browser (localStorage), keine automatische Synchronisierung

## Fachliche Hinweise

- Ein Empty-Net-Gegentor erhöht nur den Spielstand, nicht die persönliche Fangquote.
- Nur Schüsse **aufs Tor** zählen; Pfosten, vorbei und geblockte Schüsse nicht.
- Rebound/Breakaway sind Markierungen des gleichen Schusses, keine zusätzlichen Schüsse.
- Die Einsatzzeit wird manuell erfasst und kann bei falscher Eingabe ungenau sein.
- Für eine korrekte GAA muss die tatsächliche Einsatzzeit erfasst werden; 60 Minuten sind die Bezugsgröße.
- Die App ist eine Beta, kein offizielles Spielberichtssystem. Vor Live-Einsatz auf dem eigenen Gerät prüfen.

## Datenschutz / Veröffentlichung

Keine Werbung, Analyse-SDKs, Nutzerkonten oder Datenübertragung sind eingebaut. Dennoch sind für eine öffentliche Website je nach Betreiber und Hosting Impressum und Datenschutzhinweise zu prüfen. Insbesondere keine Namen Minderjähriger ohne passende Rechtsgrundlage öffentlich veröffentlichen. Diese Software ist kein fertiges Bezahlsystem. Bei Monetarisierung Hosting-Nutzungsbedingungen, Steuern, Verbraucherrecht und Zahlungsabwicklung prüfen.
