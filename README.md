# OpenCity Web

An experimental open-world city sandbox that runs entirely in your browser, built with WebAssembly and WebGPU.

> **Status:** Early prototype. Expect bugs and missing features.
https://taker.gold/five

## Disclaimer

This is an independent, fan-inspired project. It is **not affiliated with, endorsed by, or sponsored by** Rockstar Games, Take-Two Interactive, or any other game publisher. It contains **no proprietary code, assets, names, logos, or trademarks** from any commercial game. All code, models, textures, and audio in this repository are original or released under open licenses (see [Credits](#credits)).

## Features

- **WebGPU renderer** with automatic WebGL 2 fallback `[confirm]`
- **WebAssembly core** compiled from `[Rust / C++]` for game logic and physics
- **Multithreading** via Web Workers and SharedArrayBuffer `[confirm]`
- **Procedural city generation** with roads, buildings, and traffic `[confirm]`
- **Vehicle and character controller** with keyboard and gamepad support
- **Offline-friendly:** assets cached locally using IndexedDB, with saves stored in the browser
- **No installation:** runs in any modern browser with WebGPU support

## Demo

`[Link to live demo]`

`[Add screenshots or a GIF here]`

## Requirements

- A browser with WebGPU support (recent Chrome, Edge, or Firefox Nightly `[verify current support]`)
- A discrete or integrated GPU with up-to-date drivers
- Recommended: 8 GB RAM or more

## Getting Started

```bash
git clone https://github.com/[your-username]/opencity-web.git
cd opencity-web
npm install
npm run build:wasm
npm run dev
```

Open `http://localhost:5173` in your browser.

## Controls

| Action | Keyboard | Gamepad |
|---|---|---|
| Move | W A S D | Left stick |
| Look | Mouse | Right stick |
| Sprint | Shift | A / Cross |
| Enter vehicle | F | Y / Triangle |
| Pause | Esc | Start |

## Project Structure

```
/src        TypeScript front end and renderer
/engine     WebAssembly core (physics, simulation)
/assets     Original models, textures, and audio
/docs       Architecture notes
```

## Roadmap

- [ ] Day/night cycle
- [ ] Traffic AI improvements
- [ ] Touch controls
- [ ] Mod support
- [ ] `[your next goal]`

## Contributing

Contributions are welcome. Please open an issue before submitting large changes. **Do not submit code or assets taken from commercial games or from leaked or decompiled sources**, as such contributions will be rejected.

## License

Code is released under the [MIT License](LICENSE). Assets are licensed as noted in [ASSETS.md](ASSETS.md).

## Credits

- Built with `[Three.js / wgpu / Babylon.js / etc.]`
- Models and textures: `[creator, license, link]`
- Audio: `[creator, license, link]`
