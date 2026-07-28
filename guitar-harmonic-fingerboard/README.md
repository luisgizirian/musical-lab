# Guitar Harmonic Fingerboard

## Status
📋 Planned — not yet implemented.

## Goal
Visualize natural and artificial harmonics on a guitar fretboard, showing which
fret/string position produces which overtone, and animate how the string
vibrates to produce it.

## Key Features
- Display natural harmonics across the fretboard
- Display artificial harmonics (e.g., touch harmonics)
- Show nodes and antinodes for a selected harmonic
- Show which fret produces which overtone
- Animated visualization of string vibration for a selected harmonic

## Tech Stack
- C# / .NET
- [NAudio](https://github.com/naudio/NAudio) — audio capture, playback, file I/O
- [MathNet.Numerics](https://numerics.mathdotnet.com/) — FFT and DSP math
- [ScottPlot](https://scottplot.net/) — waveform/spectrum plotting and animation

## Role in the Umbrella Plan
Directly tied to guitar relearning/practice: builds guitar-specific harmonic
domain knowledge and visualization on top of the FFT/harmonic-extraction engine
from `harmonic-spectrum-explorer`, and feeds into `harmonic-practice-assistant`.
See [`/plans/harmonics-projects-plan.md`](../plans/harmonics-projects-plan.md)
for the full rationale and project order.
