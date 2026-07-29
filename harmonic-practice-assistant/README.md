# Harmonic Practice Assistant

## Status
📋 Planned — not yet implemented.

## Goal
Listen as the user practices a single note or chord (e.g., on guitar) and
provide feedback on harmonic quality and technique consistency, turning subtle
changes in technique into measurable progress over time.

## Key Features
- Real-time listening/analysis of a practiced note or chord
- Feedback: was the harmonic clean? were there unwanted overtones?
- Feedback: was the attack stable? was finger pressure consistent (proxy via
  harmonic cleanliness/stability)?
- Compare today's harmonic profile against previous sessions
- Visualize technique improvement over days/weeks

## Tech Stack
- C# / .NET
- [NAudio](https://github.com/naudio/NAudio) — audio capture, playback, file I/O
- [MathNet.Numerics](https://numerics.mathdotnet.com/) — FFT and DSP math
- [ScottPlot](https://scottplot.net/) — progress/trend visualization

## Role in the Umbrella Plan
The standout project combining guitar technique with neuroscience/motor-control
and rehabilitation-style feedback loops. Builds on the analysis engine from
`harmonic-spectrum-explorer` and the fretboard/harmonic domain knowledge from
`guitar-harmonic-fingerboard`. See
[`/plans/harmonics-projects-plan.md`](../plans/harmonics-projects-plan.md) for
the full rationale and project order.
