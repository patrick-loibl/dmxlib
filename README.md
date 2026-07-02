# XLUX-dmxlib — DMX Fixture Library

DMX fixture profile library for the XLUX lighting gateway
([XLUX-MAIN-MCU](https://github.com/patrick-loibl/XLUX-MAIN-MCU)), served via
GitHub Pages. An in-repo mirror lives at
[XLUX-shared](https://github.com/patrick-loibl/XLUX-shared)`/dmxlib`
(intentionally still named lowercase `dmxlib`).

Each fixture is a JSON file at `<manufacturer-key>/<fixture-key>.json`, e.g.
`abstract/twister-4.json`. `index.json` is the searchable catalog (manufacturers,
fixtures, modes, channel counts).

## Usage

The gateway's WebUI loads fixture detail on demand:

```
https://<user>.github.io/XLUX-dmxlib/<manufacturer>/<fixture>.json
```

It resolves a fixture in this order: user/edited fixtures (on device) →
local base library (flashed on device) → this online library. The online
library is only fetched when a fixture is not available locally and the
browser has internet access.

## Source & License

Fixture definitions originate from the
[Open Fixture Library](https://open-fixture-library.org) (OFL) and are
distributed under the MIT License. Each fixture retains its `oflURL` field
linking back to the original definition. See [LICENSE](LICENSE).
