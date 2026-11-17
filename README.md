# Schaeffler EMV: Messen. Löten. Kaffee. — v1.1.0

Inoffizielles, fiktives Retro-Lernspiel in Grün/Grau/Weiß.
Keine realen Laborpläne, Produktdaten oder normgerechten Messergebnisse.

## Starten

Lokal am PC: `index.html` im normalen Browser öffnen. Alternativ die separat
angebotene Einzeldatei `Schaeffler_EMV_Lab_v1.1.0_SPIEL.html` verwenden.
Auf dem Smartphone wird GitHub Pages / HTTPS empfohlen. Keine Installation,
kein npm, keine Bibliotheken und kein Build nötig. Grafik und Audio sind
integriert bzw. werden lokal erzeugt.

## GitHub Pages veröffentlichen

1. ZIP entpacken und ein eigenes GitHub-Repository erstellen oder öffnen.
2. Über Add file → Upload files die DATEIEN hochladen, nicht die ZIP selbst.
   `index.html`, `manifest.webmanifest` und `sw.js` gehören ins Hauptverzeichnis.
   Den Unterordner `icons` mit den zwei PNG-Dateien erhalten.
3. Die Dateien in `main` committen.
4. Settings → Pages → Build and deployment → Source:
   Deploy from a branch → main → /(root) → Save.
5. Nach erfolgreicher Veröffentlichung zeigt GitHub die echte Pages-Adresse an.
   Diese auf dem Smartphone im normalen Browser öffnen.

Offizielle Dokumentation:
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

Die Veröffentlichung wurde hier NICHT ausgeführt. Der Chat hat keinen
Schreibzugriff auf dein GitHub-Konto. Bei Firmenkonten die jeweiligen
Veröffentlichungsfreigaben prüfen. GitHub Pages ist öffentlich: keine echten
internen Labor-, Personen- oder Produktdaten hochladen.

## Smartphone / PWA

- Links den analogen Joystick ziehen, rechts Aktion antippen.
- Arbeit vortäuschen ist ein EIN/AUS-Umschalter.
- Oben links Aufgaben anzeigen. Nächster Schritt navigiert automatisch.
- Objekte oder Boden antippen: automatischer Laufweg.
- Zwei Finger auf dem Spielbereich: Pinch-Zoom. Alternativ +/− verwenden.
- Portrait / Querformat und sichere Displayränder werden berücksichtigt.
- Optional in Safari über Teilen → Zum Home-Bildschirm hinzufügen.
  Chrome bietet je nach Gerät App installieren / Zum Startbildschirm an.
- Der optionale Offline-Cache funktioniert nach dem ersten erfolgreichen Laden
  über HTTPS mit allen Dateien. Das Spiel selbst benötigt keinen Server-Code.

## Audio

Im Menü oder in den Einstellungen Sound aktivieren & testen antippen.
Hintergrundmelodie und Effekte sind standardmäßig aktiviert.
Browser verlangen eine echte Nutzerinteraktion vor der Audiofreigabe.
Bei Stille: Medienlautstärke und Stumm-Modus prüfen; normale Browseransicht
statt Chat-Vorschau / Reader-Modus verwenden. Die Einstellungen zeigen den
AudioContext-Zustand und mögliche Fehler an.
Audio verwendet Resume, eine Start-Warteschlange und einen eigenständigen
Look-ahead-Scheduler. Kein echter Geräte-/Lautsprecher-Hörtest war hier möglich.

## Desktop

WASD / Pfeile laufen · E interagiert · B halten täuscht Arbeit vor
Tab Karte · Esc Pause / Menü · Klick navigiert · Mausrad Zoom

## RE / CE Ablauf

DUT an der Ausgabe holen. Zugewiesene Kabine A/B/C betreten.
RE: Monopolantenne aufstellen.
CE: LISN / künstliches Netz vor den DUT-Tisch stellen und erneut bedienen,
um die simulierten Verbindungen zum DUT herzustellen.
Auftragsbereich am Bedienfeld einstellen; CE fordert den Peak-Demodetektor.
DUT auf den Tisch, hinausgehen, Tür schließen, Außenkonsole bedienen.
Nach Roh-FAIL: DUT mitnehmen, EMV-Filter in der Werkstatt einlöten.
Drei Timing-Treffer oder sichere automatische Montage wählen.
DUT zurückbringen und von außen nachmessen. Kollegengespräch und je nach
Auftrag Kaffee, Wartung oder Blumen erledigen. Protokoll im Büro abgeben.

CE ist didaktisch an den Automotive-Kontext von CISPR 25 angelehnt.
ALLE Pegel und Grenzlinien sind fiktiv: keine vollständige Normprüfung,
keine echten Klassengrenzwerte, keine OEM-Freigabe, keine reale Anschluss-
oder Lötanleitung. RE nutzt ein Monopol-Demoprofil.

## Laborleben

Drei Kollegen sitzen vor den Kabinen und spielen am Handy. Bei Chef-Alarm
wechseln sie in den Arbeitsmodus. Genau zwei Simulationsingenieure laufen
herum und fragen nach Messplatz, Konvergenz oder Kaffee.
In beiden Küchen wird über Wetter, E-Autos, Solaranlagen und KI geredet.
Kommt der Chef, wird plötzlich über Arbeit gesprochen oder mit
Oh, ich habe ein Meeting! an einen Arbeitsplatz geflüchtet.
Wird der Spieler unproduktiv erwischt, ist eine ZUSÄTZLICHE Messung nötig;
sie ersetzt nicht die reguläre Nachmessung. Offene Auflagen sperren das Protokoll.
Der Doktor kommt mit Erdungsring-Randbemerkungen: ausweichen, zuhören,
ins Meeting flüchten oder fachlich kontern.
Blumen können gegossen werden und trocknen im aktiven Spiel wieder aus.
Kaffeeautomaten benötigen Wasser, Bohnen, leere Kaffeeschalen und Reinigung.
Kollegen verbrauchen ebenfalls Kaffee. Einzelservice oder Alles versorgen wählen.
Wartung bleibt bei null Energie möglich; danach Kaffee laden. Kein irreversibler
Erschöpfungs-Softlock.

## Speichern / Version

Leicht 4, Mittel 6, Schwer 8 gemischte Aufgaben.
Version 1.1 nutzt eigene lokale Speicher-Schlüssel. Alte 1.0-Spielstände bleiben
erhalten, werden wegen der neuen Aufgaben aber nicht übernommen.
JSON-Export/Import in Einstellungen. Mess-CSV und Schichtbericht im Spiel.
Exit speichert und beendet die Laboransicht. Manuell geöffnete Tabs müssen
gegebenenfalls selbst geschlossen werden, wenn der Browser dies blockiert.

## Qualitätssicherung

37 automatische Prüfungen bestanden, inklusive vollständigem RE- und CE-Auftrag
mit Wegsuche, allen Kampagnen, Wartung, Pflege, Chef und Doktor sowie Touch- und
Audio-API-Tests mit Testadaptern. Kein visueller Test in einem echten Browser
und kein Hörtest auf realen Geräten. Der JSON-Testbericht enthält die Ergebnisse
und einen SHA-256-Integritätshash der eigenständigen HTML-Datei.

## Credits

Konzept / Änderungswünsche: Nutzeranfrage.
Entwicklung, Dialoge, originale Pixelgrafik und synthetischer Sound:
Schaeffler Chatbot / Data Science Solutions.
Schaeffler AG ist thematischer Kontext. Kein offizielles Unternehmensspiel
und keine freigegebene EMV-Prüfsoftware.
