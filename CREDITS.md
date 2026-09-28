# Credits & licences

These apps were built with Claude Opus 5.5. The code, data, imagery and fonts listed below come from other sources, and their licences and terms apply.

## Live data (Earth Pulse)

| Source | Used for | Terms |
|---|---|---|
| [USGS Earthquake Hazards Program](https://earthquake.usgs.gov/earthquakes/feed/) (GeoJSON summary and event-detail feeds, ShakeMap, Did You Feel It?) | Earthquakes, ShakeMap intensity images, felt-report counts | US Government public domain. Credit: U.S. Geological Survey |
| [NASA EONET v3](https://eonet.gsfc.nasa.gov/) | Wildfires, volcanoes, severe storms, sea and lake ice | NASA open data. Each event links to its upstream source (for example InciWeb, GDACS, JTWC or the Smithsonian GVP) |
| [NASA GIBS](https://nasa-gibs.github.io/gibs-api-docs/) (WMS, EPSG:4326) | "Actual view" satellite imagery: MODIS Terra and Aqua and VIIRS SNPP corrected-reflectance true colour, plus MODIS and VIIRS thermal anomalies | NASA imagery has no usage restrictions. Suggested credit: "We acknowledge the use of imagery provided by services from NASA's Global Imagery Browse Services (GIBS), part of NASA's Earth Science Data and Information System (ESDIS)." |
| [NASA Worldview](https://worldview.earthdata.nasa.gov/) | Outbound links only | NASA |
| [Where the ISS at?](https://wheretheiss.at/) (`api.wheretheiss.at`) | ISS position, altitude and velocity | Free public API. Rate limit about 1 request per second |
| [Open-Meteo](https://open-meteo.com/) | Current weather at any clicked point | Free for non-commercial use under [CC BY 4.0](https://open-meteo.com/en/license). Weather data by Open-Meteo.com |

Earth Pulse includes a bundled snapshot of the same feeds. It uses this snapshot as a fallback when a live feed can't be reached.

## Globe textures (Earth Pulse)

`earth-pulse/assets/earth-blue-marble.jpg`, `earth-night.jpg`, `earth-topology.png`, `earth-water.png` and `night-sky.png` come from the example images of the [`three-globe`](https://github.com/vasturiano/three-globe) npm package by Vasco Asturiano. The package is released under the MIT licence.

- The day, topology and water textures are derived from NASA's **Blue Marble** imagery ([NASA Visible Earth](https://visibleearth.nasa.gov/collection/1484/blue-marble)).
- The night texture is derived from NASA's **Black Marble / Earth at Night** imagery.
- NASA imagery is generally not copyrighted and can be used with credit to NASA.
- The `three-globe` README does not document where the star-field image (`night-sky.png`) comes from. It is used here as the package ships it.

## Software

- [three.js](https://threejs.org/) r170, © three.js authors, MIT licence. It is loaded from jsDelivr and includes the OrbitControls, EffectComposer, UnrealBloomPass, OutputPass, ShaderPass and FXAAShader add-ons.

## Fonts (Google Fonts, SIL Open Font License 1.1)

- Landing page: Instrument Serif, Hanken Grotesk, JetBrains Mono
- Earth Pulse: Unbounded, Hanken Grotesk, JetBrains Mono
- Agent Mission Control: Oxanium, IBM Plex Sans, JetBrains Mono

## Codebase Galaxy

The demo is a scan of [fastapi/fastapi](https://github.com/fastapi/fastapi) and its git history, and it embeds short excerpts of FastAPI source code. FastAPI is © Sebastián Ramírez and is released under the MIT licence; see [`codebase-galaxy/LICENSE-fastapi.txt`](codebase-galaxy/LICENSE-fastapi.txt). Code highlighting uses [highlight.js](https://highlightjs.org/) 11.9.0 (BSD 3-Clause), loaded from cdnjs. Fonts: Unbounded, Bricolage Grotesque and JetBrains Mono (SIL OFL 1.1).

## Agent Mission Control

The app ships with two simulated multi-agent runs set in the public [fastapi/fastapi](https://github.com/fastapi/fastapi) repository (an issue turned into a pull request, and an upgrade-research report). They are illustrations, not records of real runs. The app does not fetch any external data.
