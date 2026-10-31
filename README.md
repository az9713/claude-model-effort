# Claude Code: the (model, effort) grid

**Live page: https://az9713.github.io/claude-model-effort/**

This project is one web page. It shows when to use each pair of model and effort level in Claude Code.

## Origin

[Bart Slodyczka](https://www.youtube.com/@bartslodyczka) published the video
[Anthropic Just Told Us Which Effort Level Actually Works](https://www.youtube.com/watch?v=34J2-00SkVk).
In the video, he builds the same app at each of the five effort levels and grades each build with 17 hidden tests.
He reports that low effort took 44 seconds and cost 18 cents, and that max effort took 40 minutes and cost $9.50.
He reports the same score for both.
This project extends the video from one model to three models.

## What the page contains

- A grid of 3 models (Sonnet 5.5, Opus 5.5, Fable 5.1) by 5 effort levels (low, medium, high, xhigh, max). That is 15 cells.
- Each cell has a verdict (sweet spot, useful, situational, or unproven), when to use it, how to use it, examples, and what to watch for.
- A click on a cell shows only that card and dims the other 14 cells. The URL hash records the choice, for example `#c-opus-2`.
- Three graphics from Bart's video, redrawn in SVG: the cheat sheet, the feature-development loop, and a skill file with `effort: low`. Each caption links the video.
- A source list that links the Anthropic documentation pages and blog posts used.

## Evidence quality

- The verdicts are the author's synthesis. Anthropic does not publish them.
- Part of the documentation research reached the author as fetch summaries, not verbatim text. The page footer says so.
- No source gives effort guidance for Sonnet 5.5 beyond the cited pages. The Sonnet low, high, and xhigh cards rest on general rules.
- The Fable medium cell is marked "unproven".
- Fable security and hardware figures pool xhigh and max.

## Files

| File | Purpose |
|---|---|
| `index.html` | The page. It is one file with inline CSS, inline JavaScript, and inline SVG. It loads no external script. |
| `README.md` | This file. |

## Run it locally

Open `index.html` in a browser. No build step and no server are necessary.

## Credit

The video and its three graphics belong to Bart Slodyczka. This project is not affiliated with him or with Anthropic.
