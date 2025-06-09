# neat.sheet

Welcome to the neat.sheet public fantasy football redraft sheet generator!
This has been a project dedicated to developing an alternative to the data heavy sheets that are out there.

## What is this?

This repository contains:
- **Printable PDF draft sheets** for a multitude of league setups (roster compositions + scoring settings, etc.)
- A **community-driven configuration file** (`league_configs.json`) describing each available draft sheet
- A simple process for **requesting new league configurations**—if you don’t see your league here, request it and we’ll generate it!

Sheets are updated daily for the latest player projections and rankings

## How to Find Your Draft Sheet

1. Browse the [`/generated`](./generated) folder for the latest date.
2. Each subfolder is named for a league configuration (e.g., `ppr`, `superflex_halfppr`, etc.).
3. Download the draft sheet PDF that matches your league.
4. See [`index.json`](./index.json) or [`league_configs.yaml`](./league_configs.yaml) for details on each configuration.

## Requesting a New League Configuration

Don't see your league format? Want a custom scoring setup? You can request a custom draft sheet!

**How to request:**
- [Open an Issue](../../issues/new?template=request-config.yaml) using our "Draft Sheet Config Request" template.

**Config fields to specify:**
- Scoring system (PPR, half-PPR, standard, custom values)
- Roster composition (e.g., 1QB/2RB/3WR/1TE/1FLEX/1K/1DST, etc.)
- Any other custom settings

- ## Contributing

We welcome:
- **Config requests** for new league types
- **Feedback** on existing sheets

---

## License & Data Sources

- Generated draft sheets are provided for personal, league, and non-commercial use.
- Please see [`DATA_SOURCES.md`](./DATA_SOURCES.md) for information on where rankings and projections come from.
- All config and metadata files are open for contributions.

---

## Questions & Support

Open an [issue](../../issues) or start a [discussion](../../discussions) if you have questions or suggestions!

---

