# READYation

Radiation readiness on the astronaut visor. An interactive 3D helmet that turns solar proton flux into a visor warning.

**Live site:** https://snnnue.github.io/readyation/

## What it does
- Drag to rotate the helmet, scroll to zoom, double-click to reset
- Set the >10 MeV proton flux (1 to 100,000 pfu) or pick a real event (May 2024, Sep 2017, Mar 2012)
- The visor display changes with the level
  - below 10 pfu: green, NOMINAL
  - 10+: yellow, CAUTION
  - 100+: orange, WARNING
  - 1,000+: red, DANGER
- Astronaut view puts the camera inside the helmet so you see the warning the way the crew would

Thresholds follow NOAA's solar radiation storm scale (S1 = 10, S2 = 100, S3 = 1,000 pfu). Protons and hits are illustrative.

## Context
Part of a datathon project (NASA Track: Beyond Earth) using NASA OMNI space weather data. The analysis found that radiation storms usually arrive before geomagnetic storms, and most come with no strong geomagnetic storm at all, so crew radiation decisions should follow proton flux rather than geomagnetic alerts.

Built with three.js. Single HTML file, no build step.
