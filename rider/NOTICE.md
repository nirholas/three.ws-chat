# rider/ notice

`rider/` is derived from [Moon Rider](https://github.com/supermedium/moonrider)
by Supermedium (commit `f756aa6`, 2024-02-29), used under the MIT License in
[LICENSE](LICENSE).

## Changes from Moon Rider

- Added avatar dancing: `src/components/agent-dance.js`,
  `src/components/agent-picker.js`, `assets/dance.json`, avatar models in
  `assets/avatars/` and animation clips in `assets/clips/`.
- Added desktop controls (`src/components/desktop-input.js`) and a dual view
  (`dual.html`).
- Modified the beat, beat-generator, leaderboard, menu-mode, search and
  supercutfx-shader components, the state, colors, beatmap converter, utils,
  search index, scene, assets and news templates, the stylesheet, the
  webpack and package config, and the logos and loading images.
- Committed the webpack output (`build/`), and dropped Moon Rider's README,
  CNAME and raw design sources (`.psd`, `.blend`).

## Third-party code in vendor/

- `aframe-master.min.js` (loaded by `index.html`) is the unmodified A-Frame
  1.3.0 release build from [aframevr/aframe](https://github.com/aframevr/aframe)
  (commit `cc3516ce`), which bundles three.js r137 via `super-three`.
  `aframe-master.js` is Moon Rider's A-Frame 0.9.2 build from Kevin Ngo's
  fork (commit `154f7d07`, 2019-05-30), which bundles Supermedium's three.js
  fork (r103dev). A-Frame: MIT License, see
  [vendor/LICENSE-aframe](vendor/LICENSE-aframe).
- `BufferGeometryUtils.js`, `CatmullRomCurve3.js` and `Curve.js` from
  [three.js](https://github.com/mrdoob/three.js), adapted by Supermedium to
  the global `THREE` namespace (`Curve.js` also takes optional targets).
  three.js (these files and the copies bundled in the A-Frame builds): MIT
  License, see [vendor/LICENSE-three.js](vendor/LICENSE-three.js).
