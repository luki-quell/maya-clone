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
Alle Daten bleiben lokal im `localStorage` des Browsers (Schlüssel `luna-zyklus-daten-v1`).
Über „Mehr" → „Als JSON exportieren" kann ein Backup als JSON heruntergeladen und später wieder importiert werden.
