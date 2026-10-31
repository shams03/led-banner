# Signal

A phone-friendly LED text banner. Open `dist/index.html` in a browser, or serve `dist/` with any static server. No build or dependencies are required.

For local hosting:

```sh
python3 -m http.server 5173 --directory dist
```

Open http://localhost:5173. For use on your phone, deploy `dist/` to an HTTPS static host. Fullscreen, orientation locking, and screen wake lock depend on browser support; the full-window banner remains usable when these APIs are unavailable. Phone screen brightness is controlled through the phone's own settings.

Features: automatic text fitting, a 25–100% text-size slider, six color presets and custom color, solid or LED-dot lettering, three flash speeds or steady mode, adjustable glow, local setting persistence, and fullscreen presentation with fading controls. Text never scrolls.

JavaScript syntax and logic checks passed, including text wrapping at five viewport widths. Visual browser and physical-device verification could not be completed in the build environment.

## Deploy to Vercel

Import the GitHub repository into Vercel. Choose **Other** as the framework preset, leave the build command empty, and set the output directory to `dist`. The repository root is the project root. This is a static site and needs no server functions or backend.
