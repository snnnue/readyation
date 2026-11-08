# READYation

Radiation readiness on the astronaut visor. An interactive 3D helmet that turns solar proton flux into a visor warning.

**Live site:** https://snnnue.github.io/readyation/  
**Mission console:** https://snnnue.github.io/readyation/console/

## What it does
- Drag to rotate the helmet, scroll to zoom, double-click to reset
- Set the >10 MeV proton flux, switch on a READYation storm forecast, or step through the September 2017 storm
- The visor display uses the same tiers as the READYation mission console
  - Green CLEAR when there is no alert
  - Yellow WATCH when flux holds at 1 pfu or more for 15 minutes, or when the READYation model forecasts a storm
  - Orange STORM at NOAA S1 (10 pfu)
  - Red DANGER at NOAA S3 (1,000 pfu)
- Astronaut view puts the camera inside the helmet so you see the warning the way the crew would

Protons and hits are illustrative. The helmet shows how a READYation alert would reach a crew member. The forecasts themselves come from the READYation model (IBM Granite TinyTimeMixer r2, fine-tuned on 2010 to 2013 and tested on 2014 to 2020).

## Context
Part of a datathon project (NASA Track: Beyond Earth) using NASA OMNI space weather data. The analysis found that radiation storms usually arrive before geomagnetic storms, and most come with no strong geomagnetic storm at all, so crew radiation decisions should follow proton flux rather than geomagnetic alerts.

Built with three.js. Single HTML file, no build step.
