# Luna · Zyklus-Tracker (Maya-Klon)

Ein lokaler Zyklus-Tracker als **eine einzige Datei** (`index.html`) – reines HTML + Inline-CSS + Inline-JS, kein Backend, kein CDN.

## Starten
Einfach `index.html` doppelklicken (funktioniert auch von `file://`, komplett offline).

## Funktionen
- Übersicht: Zyklus-Tag, Phase (Menstruation / Follikelphase / Fruchtbare Phase / Lutealphase), „Periode starten“, Schnell-Symptome
- Prognose: nächste Periode, geschätzter Eisprung, fruchtbares Fenster (Ø aus dem bisherigen Verlauf, Fallback 28/5 Tage)
- Kalender mit Perioden-Markierung (Intensität), fruchtbarem Fenster, Eisprung/Prognose; Tages-Editor (Blutung 1–4, Symptome, Notiz)
- Statistik: Ø Zykluslänge, Ø Periodenlänge, Verlauf

## Datenspeicherung
- Primär: `localStorage` des Browsers (Schlüssel `luna-zyklus-daten-v1`) + `navigator.storage.persist()` gegen automatisches Löschen.
- **Unabhängig vom Browser-Cache:** unter „Mehr" → „Datei verknüpfen" eine echte `luna-daten.json` auf dem Gerät auswählen (File System Access API, Chrome/Edge). Jede Änderung wird automatisch in diese Datei geschrieben – sie übersteht auch das Löschen von Cache/Websitedaten. Auf iOS Safari stattdessen „Als JSON exportieren"/„JSON importieren" nutzen.
- Manuelles Backup jederzeit über „Mehr" → „Als JSON exportieren".
