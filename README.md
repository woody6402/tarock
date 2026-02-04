# Tarock (Königsrufen) Schreiben

Kleine, browserbasierte HTML/JS-App zum Schreiben von Tarock-Runden.  
Läuft komplett lokal im Browser – kein Backend, keine Abhängigkeiten.
Sollte auch am Handy (schmal) laufen

![Screenshot](Screenshot-20260203225935-1236x774.png)

## Features

- Unterstützung für **bis zu 6 Spieler**
- Pro Runde **genau 4 aktive Spieler**
  - Gewinner / Verlierer / Ausgesetzt
  - Bei 6 Spielern sind automatisch 2 ausgesetzt
- **Leere Spielernamen erlaubt**
  - Spieler mit leerem Namen werden **nicht angezeigt**
  - Keine Auswahlbox (G / V / –) für diese Spieler
- Ergebnis-Tabelle mit
  - aktuellem **Datum im Header**
  - Rundenergebnissen je Spieler
  - Gesamtsummen
- Automatische Punkteberechnung
- Spielstand wird im **localStorage** gespeichert

## Bedienung

1. Spielernamen eingeben  
   → leer lassen = Spieler wird ausgeblendet
2. Pro Runde genau **4 Spieler aktiv** setzen
3. Spieltyp und Punkte wählen
4. Runde schreiben
5. Letzte Runde kann rückgängig gemacht werden

## Technik

- Reines **HTML / CSS / Vanilla JavaScript**
- Keine externen Libraries
- Funktioniert offline

## Hinweise

- Spieler-UI und Ergebnistabelle passen sich dynamisch an die aktiven Spieler an
- Bei strukturellen Änderungen kann es sinnvoll sein, den `localStorage` zu leeren
