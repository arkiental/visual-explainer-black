# Visual Explainer — Black

A personal Codex skill for concise, shareable charts and explanation cards: black background, white text, and purposeful accent colors.

## Install

Copy this repository into `~/.codex/skills/visual-explainer/`, preserving or backing up any existing skill first. Invoke `$visual-explainer` with the data you want explained. The skill produces a PNG and editable HTML.

The three PNGs in `references/examples/` are user-supplied design references. They are included for private agent reference; no ownership or redistribution rights are asserted. The skill explicitly instructs agents to inspect a relevant image before designing.

This is a focused personal adaptation of the visual-explanation workflow introduced by [nicobailon/visual-explainer](https://github.com/nicobailon/visual-explainer). Its instructions were rewritten for this user's compact black-background card style. This repository does not bundle the upstream runtime, commands, or templates.

## Required font

Futura is mandatory for all output typography. Font files are not yet bundled: none were available locally when this requirement was added. Supply Futura files licensed for repository inclusion, with their license, in assets/fonts/. The agent must not silently substitute a different font.

