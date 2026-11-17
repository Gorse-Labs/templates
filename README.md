# Gorse Labs templates

Free device templates for Loxone and other smart building systems, by [Gorse Labs](https://gorselabs.com/templates).

Each device starts as one checked register map (addresses, scaling, units, value meanings, where it was tested). Templates for each system are built from that map, so a fix made once reaches every system. Loxone comes first; Home Assistant and ESPHome are next.

## Status labels

| Label | Meaning |
| --- | --- |
| Wanted | On the list, not started |
| In build | Being written |
| Unverified (beta) | Built from the maker's documents, not yet proven on real kit |
| Community tested | Passed the test checklist on at least two sites, firmware listed |
| Gorse verified | Tested by Gorse Labs on real kit |

Everything in [`beta/`](beta) is **v0.1, unverified**. Check every reading in the Loxone Modbus Monitor before using it in logic.

## What's here

| Device | System | File | Status |
| --- | --- | --- | --- |
| Mitsubishi Ecodan (MelcoBEMS MINI A1M/A1M+) | Loxone | [Monitor](beta/loxone/mitsubishi-ecodan) | Beta, read only |
| SolarEdge inverter | Loxone | [Gorse edition](beta/loxone/solaredge) | Beta, read only |
| Daikin Altherma via HomeHub (EKRHH) | Loxone | [Monitor](beta/loxone/daikin-altherma-homehub) | Beta, read only |

Only read-only (Monitor) templates are published while in beta. Control templates write to the device, so they go to signed-up testers first and are published once they pass testing.

## Import into Loxone Config

1. Download the raw `MB_*.xml` file.
2. In Loxone Config, select your Modbus Extension (RTU) or Modbus Server (TCP) in the Periphery tree, then Device Templates → Import Template.
3. Set the device address and serial settings (RTU) or IP and port (TCP), then check readings in the Modbus Monitor.

## Help test

Got one of these devices? Sign up as a tester at [gorselabs.com/templates](https://gorselabs.com/templates). Testers are credited in the template.

Found a wrong register or scaling? Open an issue with your device model, firmware and what you saw.

## Licence and credits

Templates are licensed under [CC BY 4.0](LICENSE): free to use, including on paid jobs, with credit to Gorse Labs. Some templates build on other people's work; see [CREDITS.md](CREDITS.md).

Templates are AI-assisted and provided as-is, without warranty. Test before relying on them.
