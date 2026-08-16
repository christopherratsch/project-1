# 80. Geburtstag – Schloss Steinburg, Würzburg

Kleine Web-App zur Organisation der Geburtstagsfeier am 22.–23. August 2026.

Alles steckt in einer einzigen Datei: [`index.html`](index.html). Kein Server,
keine Datenbank – einfach im Browser öffnen.

## Funktionen

- **Gästeliste** – Name, Zusage-Status (zugesagt / offen / abgesagt),
  Übernachtung und Anmerkungen (z. B. Diätwünsche). Oben die Zähler für
  Gesamt, Zugesagt und Übernachtungen. Status und Übernachtung lassen sich
  direkt in der Liste ändern.
- **Ablaufplan** – Programmpunkte mit Uhrzeit, Titel, Ort und Verantwortlichem,
  getrennt nach Tag 1 (22.8.) und Tag 2 (23.8.), automatisch chronologisch sortiert.
- **To-dos** – Checkliste mit Fälligkeitsdatum; überfällige Aufgaben werden markiert.
- **CSV-Export** der Gästeliste (Semikolon-getrennt, mit BOM – öffnet sich
  direkt in Excel), z. B. für das Hotel.

## Daten

Alle Eingaben liegen im `localStorage` des Browsers – sie bleiben also nach dem
Schließen erhalten, sind aber an genau diesen Browser auf diesem Gerät gebunden
und werden nirgendwohin übertragen. Für ein Backup den CSV-Export nutzen.
