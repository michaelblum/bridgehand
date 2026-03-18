# Bridgehand

Bridgehand is a small browser prototype repo. This particular experiment centers on Slippy: a deliberately conspicuous, slightly goofy character that riffs on Clippy while testing what it feels like to give an agent a visible presence inside a page.

This is not meant to present a complete product vision, or even my most developed version of this general idea. It is one playful branch of a broader line of thinking about browser-side agent interfaces. Some of my other experiments are much less character-driven and much more utility-focused.

This repo exists because the experiment was fun, useful, and concrete enough to keep around.

## What is in here

The current prototype includes:

- A draggable on-page character with eye tracking, pose changes, and pointing behavior.
- Speech bubbles, tails, and layout logic that react to viewport and target changes.
- Highlighting and guided-tour style overlays.
- A small control surface for tuning and debugging placement behavior.
- A standalone file-based setup with no build step.

## Why Slippy

Slippy is intentionally a little loud. The character design leans into the joke of an overly noticeable assistant, which makes it a decent vehicle for testing how much presence is too much, how motion reads in a workspace, and when a helper starts to feel intrusive instead of useful.

That is part of the point of this repo: it is a sketchpad for trying ideas quickly, not a final answer.

## How it came together

This was very much a learning-by-doing project. Different parts were prototyped or refined with different tools:

- Google Gemini Canvas helped get the mini app moving early.
- Codex was used heavily for iteration, debugging, and implementation.
- Some of the character art and cleanup work were generated or assisted with AI tools.

So the repo is also a record of that process: a small experimental app that grew through a mix of hand-editing, tool-assisted prototyping, and lots of iteration.

## Repo layout

- [`index.html`](./index.html): the standalone prototype.
- [`index.prev.html`](./index.prev.html): an earlier snapshot kept for comparison.
- [`assets/`](./assets): local art and arm assets used by the demo.
- [`_unused/`](./_unused): scratch and reference files that came along with the experiment.

## Running it

Open [`index.html`](./index.html) in Chrome.

- No install step.
- No build step.
- No server required.

Drag Slippy, the bubble, or the control panel around and click through the demo states.

## Notes

If you are looking for the polished or more utility-heavy version of this line of work, this is not that. This repo is the playful one.
