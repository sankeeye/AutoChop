# AutoChop

Een simpel automation-script voor Roblox lumber-games. Truck rijdt automatisch pulserend vooruit en chopt continu met Q. Geen computer vision nodig, geen complexe setup.

## Download

**[Laatste versie](https://github.com/sankeeye/AutoChop/releases/latest)**

## Wat doet het

- W wordt pulserend ingedrukt (default: 0.20s gas / 3.20s wachten)
- Q wordt elke 250ms gedrukt — de game chopt automatisch als er een boom in range is
- Draaien doe je zelf met A/D
- Snelheid is in real-time tunebaar via hotkeys

## Installatie

1. Download `AutoChop.zip` van de [releases pagina](https://github.com/sankeeye/AutoChop/releases/latest)
2. Pak de map ergens uit (bijv. bureaublad)
3. Rechtsklik `start.bat` → "Als administrator uitvoeren"
4. Eerste keer: klik "Ja" op de admin-popup. Python en de benodigde packages worden automatisch geïnstalleerd (vereist internet).
5. Volgende keren: dubbelklik `start.bat`, overlay verschijnt direct.

## Gebruik

1. Open je Roblox lumber-game, ga in je truck
2. Druk **F6** om AUTO te starten
3. Tune indien gewenst met de hotkeys (zie hieronder)

## Hotkeys

| Toets | Functie |
|-------|---------|
| **F6** | AUTO aan/uit |
| **PgUp** | Wacht-tijd +0.1s (truck langzamer) |
| **PgDn** | Wacht-tijd -0.1s (truck sneller) |
| **F3** | Gas-tijd +0.1s |
| **F4** | Gas-tijd -0.1s |
| **F8** | Script volledig stoppen |

## Vereisten

- Windows 10 / 11
- Internet (bij eerste run, voor Python install)
- Admin rechten (voor globale keyboard hooks)

## Bestanden in de release

- `auto_chop.py` — het Python script
- `start.bat` — auto-installer + launcher
- `LEESMIJ.txt` — beknopte instructies (Nederlands)
- `LICENSE` — MIT licentie

## Disclaimer

Externe automation van Roblox kan tegen de Terms of Service zijn. Hyperion (Roblox' anti-cheat) kan synthetische input detecteren. Gebruik op eigen risico, het liefst niet op accounts die je belangrijk vindt.

## License

MIT
