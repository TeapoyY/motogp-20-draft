# 🏎️ 17-0: IndyCar Draft — Can You Go Undefeated?

> **Draft 5 IndyCar legends across 6 eras and try to win every race in a 17-race IndyCar season.**
> 84 legends. 6 eras. 17 races. 1 goal: 17-0.

A 1-day HTML MVP sports-draft game, in the lineage of:
- 🏆 [**38-0 Football Squad Draft**](https://github.com/TeapoyY/squad-draft-football) — NFL X-0 (2026-07-30)
- 🏎️ [**F1 24-0**](https://github.com/TeapoyY/squad-draft-football) — F1 X-0 (2026-08-01)
- 🏁 [**36-0 NASCAR Cup Draft**](https://github.com/TeapoyY/nascar-36-draft) — NASCAR X-0 (2026-08-17)
- 🚛 [**24-0 NASCAR Truck Draft**](https://github.com/TeapoyY/nascar-truck-24-draft) — NASCAR Truck X-0 (2026-08-21)
- 🎮 [**PixelGP**](https://github.com/TeapoyY/app-pixelgp-web) — Turn-based racing + cards (2026-06-25)

## 🎮 How to Play

1. **Open `index.html`** in any modern browser (no build step, no dependencies)
2. **Draft 5 IndyCar legends** from across the 6 eras (1980s → 2026)
   - Mix eras to unlock **Era Synergy bonus** (+1.5 OVR per extra driver from same era)
3. **Start the season** — your highest-OVR driver is your primary for all 17 races
4. **Simulate race-by-race** — win/lose is determined by OVR + track-type + variance
5. **Crown a champion** — go 17-0 or fall short

## 🏟️ IndyCar Track Types

IndyCar has 3 distinct disciplines — the best drivers must master all:
- **Oval (5 races)**: Indianapolis 500, Iowa, Gateway, Milwaukee, Nashville — pack racing + drafting
- **Road (8 races)**: Thermal Club, Barber, Indy RC, Road America, Laguna Seca, Mid-Ohio, Portland, Monterey — skill-pure
- **Street (4 races)**: St. Pete, Long Beach, Detroit, Toronto — walls + chaos

The Indianapolis 500 (race #5) awards **DOUBLE POINTS** — this is the biggest single-race prize in motorsport.

## 📊 Difficulty Curve (Monte Carlo Verified)

200 simulated seasons per OVR (Node-validated):

| OVR | Avg Wins / 17 | Perfect 17-0 Rate | Experience |
|-----|---------------|-------------------|------------|
| 70  | 0.0           | 0.0%              | Backmarker — fighting to stay on lead lap |
| 80  | 0.0           | 0.0%              | Mid-pack — occasional top-10 |
| 85  | 0.01          | 0.0%              | Lower midfield |
| 90  | 2.6           | 0.0%              | Title contender dark horse |
| 95  | 12.8          | 0.5%              | Champion-tier — needs luck for 17-0 |
| 99  | 16.7          | 74.0%             | GOAT-tier (Palou/Dixon/Mears/Zanardi) — 17-0 is real |

## 🌟 Era Roster (84 legends, 6 eras × 14 drivers)

| Era | Decade | Notable Drivers | Era Tier |
|-----|--------|-----------------|----------|
| 1   | 1980s  | Rick Mears, Mario Andretti, Emerson Fittipaldi | Pioneers |
| 2   | 1990s  | Alex Zanardi, Michael Andretti, Paul Tracy | CART Peak |
| 3   | 2000s  | Scott Dixon, Hélio Castroneves, Dan Wheldon | IRL/CART Reunification |
| 4   | 2010s  | Scott Dixon, Josef Newgarden, Will Power | Modern Era |
| 5   | 2020s  | Alex Palou, Pato O'Ward, Colton Herta | Palou Era |
| 6   | 2026   | Alex Palou, Scott Dixon, Josef Newgarden | Active |

## 🎯 The Goal: 17-0

To go undefeated, you need:
- **Best OVR ≥ 95** driver (era-synergized roster)
- **No bad luck on 5 oval races** (drafting chaos)
- **Win the Indianapolis 500** (race #5, double points)

The best rosters can pick 4× OVR 99 legends + 1× era-synergized teammate for +1.5 OVR → 100+ effective OVR. But 17 races means **a single P3 finish breaks your perfect season**.

## 🛠️ Tech

- **0 dependencies**, single HTML file (~38KB)
- **Vanilla JS** with **mulberry32 seeded RNG** for replayability
- **LocalStorage** not required (single-session MVP)
- **Mobile-first responsive** (works on iPhone/Android browsers)

## 🧬 Lineage

This game is the 5th in the X-0 Sports Draft series:
- **NFL 38-0** (7/30) — first X-0 template
- **F1 24-0** (8/1) — refined mechanics
- **NASCAR 36-0** (8/17) — multi-track-type system proven
- **NASCAR Truck 24-0** (8/21) — small-roster variant
- **IndyCar 17-0** (8/22) — first non-stock-car racing series (open-wheel + road/oval/street)

Each iteration adds a wrinkle (era synergy, track-type modifiers, double-points events) while keeping the core X-0 viral narrative intact.

## 📦 Run Locally

```bash
git clone https://github.com/TeapoyY/indycar-17-draft
cd indycar-17-draft
open index.html  # or just double-click in Finder
```

No build, no install, no dependencies.

## 📝 License

MIT — fork, modify, ship your own X-0 variant.

---

*Built as part of the [appdailydrop](https://github.com/TeapoyY) pipeline — daily hot-app discovery → 1-day HTML MVP → GitHub push.*

*IndyCar legend data: Wikipedia + Racing-Reference.net. Track names: 2026 IndyCar Series schedule. OVR scores are author-estimated for game balance.*