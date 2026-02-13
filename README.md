# Football Tactics Base (`jaivaltamboli-pixel.github.io`)

Static website focused on football tactics, interactive explainers, and mini simulators.

## Repository structure

```text
.
├── index.html                       # Main landing page
├── possession.html                  # Possession overview page
├── defense.html                     # Defensive tactics overview
├── finesse.html                     # Finishing: finesse shots
├── power-shot.html                  # Finishing: power shots
├── whip.html                        # Crossing technique page
├── game.html                        # Training/game interaction page
├── penaltyshooter.html              # Penalty shooter simulator
├── tactics_console.html             # Interactive tactics console
├── PeripheralVision.html            # Peripheral vision training page
├── defense-types/
│   ├── counterpressing.html
│   └── low-block.html
├── possession/
│   └── positionalplay.html
├── images/                          # Shared image assets
├── robots.txt
├── sitemap.xml
└── favicon.png
```

## Navigation/linking convention

To keep nested pages reliable, internal links use **root-relative paths** (example: `/index.html`, `/defense.html`, `/possession/positionalplay.html`).

## Local preview

Because this is a static site, you can run a simple local server:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Publishing

This repository is structured for GitHub Pages deployment from the default branch.
