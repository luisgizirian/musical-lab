# Physics of Music

## Status
📋 Planned — not yet implemented.

## Goal
A larger educational application that combines multiple harmonics/acoustics
modules into a single, cohesive experience blending software engineering,
music, mathematics, and visualization.

## Key Modules
- Waves and interference
- Harmonic series
- Fourier analysis
- Instrument timbre
- Guitar harmonics
- Piano harmonics
- Chords and consonance
- Tuning systems (equal temperament, just intonation, Pythagorean tuning)
- Resonance and standing waves
- Audio synthesis
- Spectral analysis
- Interactive experiments

## Tech Stack
- C# / .NET
- [NAudio](https://github.com/naudio/NAudio) — audio capture, playback, file I/O
- [MathNet.Numerics](https://numerics.mathdotnet.com/) — FFT and DSP math
- [ScottPlot](https://scottplot.net/) — waveform/spectrum/spectrogram visualization

## Role in the Umbrella Plan
The grand unifying vision, built last so it can reuse/reference the engines and
lessons learned from `harmonic-spectrum-explorer`, `guitar-harmonic-fingerboard`,
and `harmonic-practice-assistant` as modules rather than rebuilding them from
scratch. See [`/plans/harmonics-projects-plan.md`](../plans/harmonics-projects-plan.md)
for the full rationale and project order.
