# XLUX-dmxlib — DMX Fixture Library

DMX-Fixture-Profile für das XLUX-Gateway ([XLUX-MAIN-MCU](https://github.com/patrick-loibl/XLUX-MAIN-MCU)),
ausgeliefert via GitHub Pages. Reines JSON-Datenrepo, kein Build.

## Struktur

- `<manufacturer-key>/<fixture-key>.json` — ein Fixture-Profil (z.B. `abstract/twister-4.json`)
- `index.json` — durchsuchbarer Katalog (Hersteller, Fixtures, Modes, Kanalzahlen)

## Nutzung

Die WebUI lädt Fixture-Details on-demand:
`https://<user>.github.io/XLUX-dmxlib/<manufacturer>/<fixture>.json` —
Auflösungsreihenfolge: Gerät (user/edited) → lokale Basis-Lib (geflasht) → online.
In-Repo-Mirror: `XLUX-shared/dmxlib` (bleibt klein geschrieben).

## Quelle & Lizenz

Fixtures aus der [Open Fixture Library](https://open-fixture-library.org) (MIT),
`oflURL` je Fixture verlinkt zurück. Siehe [LICENSE](LICENSE).
