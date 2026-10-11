# Tabla Beat Sequencer

A browser-based tabla rhythm sequencer for creating, editing, and playing Indian
rhythmic patterns. The app uses the Web Audio API to synthesize tabla bols in
real time, so it does not require audio samples or a backend service.

## Live demo

The project is hosted on Cloudflare Pages:

**[tabla-sequencer.pages.dev](https://tabla-sequencer.pages.dev)**

## Features

- Play and stop patterns with a visual playhead.
- Edit individual tabla strokes in the step sequencer.
- Adjust tempo from 40 to 480 BPM.
- Add swing from 0% to 50%.
- Work with different cycle lengths, including 6, 7, 8, 10, and 16 beats.
- Start from taal presets:
  - Teentaal (Teen Taal)
  - Jhaptaal
  - Rupak
  - Dadra
  - Keherwa
  - Funky Tabla
- Clear a pattern or generate a random pattern.
- Copy a pattern to the clipboard and import it again later.
- Use the app directly in a modern browser without installing dependencies.

## Getting started

### Use the hosted version

Open [tabla-sequencer.pages.dev](https://tabla-sequencer.pages.dev) in a
browser. Click the play button or an individual step to allow the browser to
start audio playback.

### Run locally

This is a static web app. Clone the repository and serve the project directory
with any local HTTP server:

```bash
git clone https://github.com/scgon/tabla-beat-sequencer.git
cd tabla-beat-sequencer
npx serve .
```

Then open the local URL shown by the server.

Opening `index.html` directly may also work, but using a local server provides
the most consistent browser behavior.

## How to use

1. Select a taal preset, or begin with the default pattern.
2. Click cells in the sequencer grid to enable or disable tabla strokes.
3. Set the tempo, swing, and cycle length using the controls at the top.
4. Press **Play** to hear the pattern and follow the active beat.
5. Use **Copy Pattern** to save a pattern as text, then use **Import Pattern**
   to restore it.

## Technology

- HTML
- CSS
- Vanilla JavaScript
- Web Audio API

The complete application, including its JavaScript, is contained in
[index.html](/Users/shaan/CodingProjects/WebstormProjects/tabla-beat-sequencer/index.html).

## Development

There is no build step or runtime dependency. Make changes to `index.html` and
reload the page in a browser to test them. The repository includes an npm test
placeholder, but the project currently has no automated test suite.
