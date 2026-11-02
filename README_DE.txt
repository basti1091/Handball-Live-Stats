HANDBALL LIVE STATS – iPhone Vollbild-/Offline-Version

WAS ENTHALTEN IST
- index.html: die Handball-App
- manifest.json: Name, Symbol und Vollbild-/Standalone-Modus
- sw.js: Offline-Speicherung der App-Dateien
- icon-192.png und icon-512.png: App-Symbole

WICHTIG
Damit der Vollbildmodus und der Offline-Betrieb auf dem iPhone funktionieren,
muss dieser Ordner über eine HTTPS-Adresse veröffentlicht werden. Eine lokal
geöffnete HTML-Datei oder ein ZIP kann keinen Service Worker installieren.

KOSTENLOSER WEG MIT GITHUB PAGES
1. Auf github.com kostenlos anmelden.
2. Ein neues Repository erstellen, z. B. handball-live-stats.
3. Alle Dateien aus diesem Ordner direkt in das Repository hochladen.
4. In Settings > Pages bei Build and deployment "Deploy from a branch" wählen,
   Branch "main" und Ordner "/ (root)" einstellen und speichern.
5. Die angezeigte HTTPS-Adresse auf dem iPhone in Safari öffnen.
6. Teilen-Symbol > Zum Home-Bildschirm > Hinzufügen.
7. Die App anschließend über das neue Home-Bildschirm-Symbol starten.

Dann startet die App ohne Safari-Adressleiste und ohne ChatGPT-Leiste. Nach dem
ersten vollständigen Laden funktioniert die App auch offline.

TORHÜTER-AUSWERTUNG
Torhüter werden separat von Feldspielern ausgewertet. Die Haltequote berechnet
sich aus Paraden / (Paraden + Gegentore). „Wurf daneben“ wird separat gezählt
und nicht in die Haltequote eingerechnet. Zusätzlich wird bei Torhütern eine Plus-/Minus-Bilanz für ihre Aktionen angezeigt.
„Technischer Fehler“ ist eine negative Aktion für alle Spieler.

DATEN
Spieler und Statistiken werden lokal auf dem iPhone im App-Browser gespeichert.
Sie werden nicht automatisch zwischen Geräten synchronisiert. Im Bereich „Kader“ über „Sicherung exportieren“ regelmäßig eine vollständige JSON-Sicherung
erstellen. Sie enthält Kader, gespeicherte Spiele und das aktuell offene Spiel. Über
„Sicherung importieren“ kann diese Datei wiederhergestellt werden. Der Import ersetzt
die aktuell gespeicherten App-Daten. Die Sicherungsdatei deshalb separat aufbewahren.

TRACKING-ANSICHT
Die Spielerauswahl zeigt fünf kompakte Spalten mit Spielerfeldern im Verhältnis 4:3.


NEU IN VERSION 5: Vor jedem Spiel unter „Spiele“ ein neues Spiel vorbereiten, Gegner und Datum eintragen und die anwesenden Spieler auswählen. Im Live-Spiel erscheinen anschließend ausschließlich diese Spieler. Die Auswahl wird mit dem Spiel gespeichert und beim Öffnen eines gespeicherten Spiels wiederhergestellt.


NEU IN VERSION 6
- Spieler im Kader bearbeiten (Name und Rückennummer).
- Vollständige JSON-Datensicherung für Kader, Spiele und offenes Spiel exportieren.
- Sicherungsdatei später wieder importieren; der Import ersetzt den aktuellen Datenbestand.
- Cache-Version aktualisiert, damit veröffentlichte Änderungen neu geladen werden.
