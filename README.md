# Neap Tide Forecasts

A concept landing page for an imaginary tide and swell app. Every animation on it is a recipe from [motion-anything](https://github.com/nexu-io/motion-anything), an open-source motion library.

**Live page:** https://4waiz.github.io/neap/

Press **M**, or the Motion notes button in the corner, to label every recipe on the page. The panel shows the motion budget for the section you're viewing (one loop, one attention moment and at most three entrances at once, from motion-anything's MOTION-SPEC) and lists what was left out and why.

## What's on the page

- 11 recipes: waves, blur-text, fade-in-up, count-up, decrypted-text, magnetic-button, elastic-slider, scroll-reveal, spotlight-card, like-burst and rotating-text.
- A tide chart computed from a sample tide curve. Drag across the day and one spring (stiffness 300, damping 30, the spec's `spring-snappy`) moves the marker, the slider and the water level on a tide staff.
- Light and dark themes. Dark mode follows the night palette of an electronic chart display.
- A reduced-motion fallback for every animation, plus a button that pauses the looping ones.

It is a single `index.html` with no build step. The only outside request is Google Fonts.

## Notes

- Gull Reef, Salt Steps, Harrow Point and Lantern Bay are invented, and every reading is sample data.
- Building this page turned up six bugs in the library's recipes. The fixes were sent upstream in [nexu-io/motion-anything#8](https://github.com/nexu-io/motion-anything/pull/8).

## Credits and license

Motion recipes come from motion-anything by nexu.io (Apache-2.0). See [NOTICE](NOTICE). This repository is licensed under the Apache License 2.0; see [LICENSE](LICENSE).
