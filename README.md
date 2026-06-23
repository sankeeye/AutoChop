# AutoChop

Een simpel automation-script voor Roblox lumber-games. Truck rijdt automatisch pulserend vooruit en chopt continu met Q. Geen computer vision nodig, geen complexe setup.

## Download

**[⬇ Laatste versie (v1.4) — Standalone .exe](https://github.com/sankeeye/AutoChop/releases/latest)**

Eén bestand. Geen Python install. Dubbelklikken en spelen.

## Wat doet het

- W wordt pulserend ingedrukt (default: 0.20s gas / 3.20s wachten)
- Q wordt elke 250ms gedrukt — de game chopt automatisch als er een boom in range is
- Draaien doe je zelf met A/D
- Snelheid is in real-time tunebaar via hotkeys
- **Instellingen worden opgeslagen** — één keer tunen, daarna nooit meer
- **Pauze-knop (F7)** — tijdelijk stoppen zonder dat de timer doorloopt
- **Geluidssignaal** als de auto-stop timer afloopt — handig bij AFK
- **Auto-update check** — script meldt automatisch als er een nieuwere versie is
- Overlay kan verborgen worden tot een klein bolletje (groen = aan, geel = pauze, rood = uit)
- **Auto-stop timer**: stopt automatisch na 15 min (instelbaar)

## Antivirus waarschuwing

Windows Defender kan AutoChop.exe ten onrechte als malware flaggen. Dit is een **false positive** omdat Nuitka-compiled .exes met keyboard hooks vaak verdacht lijken voor antivirus-software. Het is **veilig**.

Om door te gaan bij de SmartScreen-popup:
1. Klik **"Meer info"**
2. Klik **"Toch uitvoeren"**

Of voeg `AutoChop.exe` toe aan je Defender-uitsluitingen.

## Installatie

1. Download `AutoChop.exe` van de [releases pagina](https://github.com/sankeeye/AutoChop/releases/latest)
2. Dubbelklik het bestand (klik door SmartScreen-waarschuwing heen indien getoond)
3. Klik "Ja" op de UAC-popup (admin rechten nodig voor keyboard hooks)
4. Overlay verschijnt linksboven, druk **F6** om te starten

Geen Python install nodig. Geen pip. Geen zip uitpakken. Eén bestand, klaar.

## Gebruik

1. Open je Roblox lumber-game, ga in je truck
2. Druk **F6** om AUTO te starten (timer begint te lopen, default 15 min)
3. Tune indien gewenst met de hotkeys (zie hieronder) — instellingen blijven bewaard
4. Druk **F10** om de info-overlay te verbergen — alleen een klein gekleurd bolletje blijft over
5. Druk **F7** voor pauze (zonder timer reset)
6. Na 15 minuten stopt AUTO automatisch met geluidssignaal

## Hotkeys

| Toets | Functie |
|-------|---------|
| **F6** | AUTO start/stop (reset timer) |
| **F7** | PAUZE aan/uit (timer pauzeert ook) |
| **F10** | Volledige overlay verbergen / tonen (laat alleen status-bolletje zien) |
| **F11** | Download-pagina openen (bij update beschikbaar) |
| **F1** | Max-runtime +1 minuut |
| **F2** | Max-runtime -1 minuut |
| **PgUp** | Wacht-tijd +0.1s (truck langzamer) |
| **PgDn** | Wacht-tijd -0.1s (truck sneller) |
| **F3** | Gas-tijd +0.1s |
| **F4** | Gas-tijd -0.1s |
| **F8** | Script volledig stoppen |

## Bolletje-kleuren

| Kleur | Betekenis |
|-------|-----------|
| 🟢 Groen | AUTO actief en draait |
| 🟡 Geel | Gepauzeerd (F7) |
| 🔴 Rood | AUTO uit |

## Vereisten

- Windows 10 / 11
- Admin rechten (voor globale keyboard hooks)
- Internet (alleen voor update-check; werkt ook offline)
- ~10 MB schijfruimte

## Disclaimer

Externe automation van Roblox kan tegen de Terms of Service zijn. Hyperion (Roblox' anti-cheat) kan synthetische input detecteren. Gebruik op eigen risico, het liefst niet op accounts die je belangrijk vindt.

## License

MIT
