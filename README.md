# Bridgehand

Bridgehand is a proof-of-concept lab for embodied browser agents: a place to prototype what it feels like when a language-model collaborator is not just a chat box off to the side, but a visible working presence inside the shared interface itself.

The premise is simple: collaboration improves when intent becomes legible. A human partner should be able to see where the agent is looking, what it is responding to, what it is trying to point at, and which part of the workspace currently has its attention. Bridgehand explores that thesis by giving the agent a persona, a body, motion, gaze, gesture, highlighting, and a persistent control surface that all live in the browser alongside the human.

In that sense, this repo is less a character demo than a harness for alignment-by-presence. It treats embodiment as a practical interface layer: a familiar touchpoint metaphor that helps bridge the gap between model output and human understanding by making attention, intention, and action spatially explicit.

The current prototype includes:

- A browser-native avatar persona, currently expressed as Slippy.
- Eye tracking and pose changes that make the agent's focus visible.
- Speech-bubble and tail-placement logic that can respond to changing layout conditions.
- Tour-target highlighting and on-page guidance overlays.
- A control surface for tuning behavior and inspecting placement decisions.
- A standalone, file-based setup for fast experimentation without a build step.

This repository is meant to be a workshopping ground for ideas such as:

- How an agent should signal focus before it acts.
- How motion, gaze, and gesture can clarify intent.
- How an on-page UI surface can support collaboration without competing with the workspace.
- How an avatar system can act as a practical harness for browser-side agent behavior.

## Why this exists

Most LM interfaces still ask people to infer intent from text alone. Bridgehand explores a different interaction model: the agent shares the same visual field as the user, inhabits the same workspace, and exposes its internal direction of attention through motion and spatial cues. The goal is not decoration. The goal is better alignment, clearer handoffs, and more intuitive collaboration.

## Current structure

- [`index.html`](./index.html): standalone prototype surface and control panel.
- [`index.prev.html`](./index.prev.html): earlier snapshot retained for comparison.
- [`assets/`](./assets): local avatar art and arm assets.
- [`_unused/`](./_unused): source and scratch artifacts kept for reference.

## Running locally

Open [`index.html`](./index.html) in Google Chrome.

- No server, package install, or network dependency is required.
- The prototype is designed to run directly from `file://`.
- Drag Slippy, the bubble, or the control panel to workshop layout behavior.

## Status

Bridgehand is intentionally a prototype harness, not a polished product. The point is to make it cheap to test ideas about embodied agent behavior in a real browser workspace and keep iterating toward a system where a human and an LM agent can work side by side with more clarity, more shared context, and less guesswork.
