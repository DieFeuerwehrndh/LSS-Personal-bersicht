# LSS Personalübersicht - Vollversion

Unser Discord Server https://discord.gg/pWXSYEYRAu

Ein Userscript für [Leitstellenspiel.de](https://www.leitstellenspiel.de/), das eine **dragbare und resizable Personalübersicht** bietet. Alle Gebäude, exakte Fahrzeugzählungen, Filter, Sortierung, Auto-Refresh und CSV-Export inklusive.

---

## Funktionen

- Übersicht aller Wachen mit aktuellem Personal und benötigtem Personal
- Exakte Fahrzeugzählung pro Wache
- Filter: alle Wachen / nur Defizit / nur gedeckt
- Sortierung nach Name, Personal, Personal-Defizit oder Anzahl Fahrzeuge
- Suchfunktion für Wachen oder Fahrzeugtypen
- Dragbares & resizables Fenster
- Auto-Refresh mit einstellbarem Intervall
- Export der Übersicht als CSV
- Speichert Position, Größe, Filter und Sortierung im Browser-Storage

---

## Installation

1. Browser-Erweiterung installieren, die Userscripts unterstützt, z.B.:
   - [Tampermonkey](https://www.tampermonkey.net/)
   - [Violentmonkey](https://violentmonkey.github.io/)
2. Neues Userscript anlegen und den gesamten Code aus dieser Datei einfügen.
3. Speichern und die Seite [Leitstellenspiel.de](https://www.leitstellenspiel.de/) laden.
4. Button `P` in der linken oberen Ecke anklicken, um die Personalübersicht zu öffnen.

---

## Konfiguration

Im Script lassen sich folgende Parameter anpassen:

- `CFG.vehiclesLimitPerPage` – maximale Fahrzeuge pro API-Request
- `CFG.autoRefreshMs` – Standard-Auto-Refresh-Intervall (ms)
- `CFG.defaultWidthPercent`, `CFG.defaultHeightPercent` – Standardgröße des Fensters
- `CFG.minWidthPx`, `CFG.minHeightPx` – minimale Fenstergröße

Alle weiteren Einstellungen werden automatisch gespeichert (Position, Größe, Filter, Sortierung).

---

## Bedienung

- **Drag & Resize:** Fenster verschiebbar und vergrößer-/verkleinerbar  
- **Minimieren / Schließen:** Buttons im Header  
- **Suche / Filter / Sortierung:** Linkes Panel  
- **Auto-Refresh:** Aktivierbar, Intervall einstellbar  
- **CSV Export:** Aktuelle Ansicht herunterladen

---

## Lizenz

MIT License – siehe LICENSE-Datei

---

## Hinweise

- Das Script verwendet die internen LSS-APIs (`/api/buildings` und `/api/v2/vehicles`)  
- Falls Fahrzeuge nicht korrekt geladen werden, kann ein Fallback auf die ältere API (`/api/vehicles`) greifen  
- Entwickelt für Desktop-Browser, optimiert für Chrome/Firefox
