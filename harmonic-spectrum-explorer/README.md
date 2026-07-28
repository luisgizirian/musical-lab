# Harmonic Spectrum Explorer

## Status
📋 Planned — not yet implemented.

## Goal
Load an audio signal (from a file or the microphone) and analyze/visualize its
harmonic content: fundamental frequency, harmonics, relative amplitudes,
spectrogram, and waveform.

## Key Features
- Load audio from a file or record from the microphone
- Detect fundamental frequency via FFT
- Extract and display harmonics (2nd, 3rd, 4th, ...) with relative amplitudes
- Waveform and spectrogram visualization
- Play back individual harmonics in isolation
- Mute selected harmonics
- Reconstruct the sound after removing selected harmonics
- Compare harmonic content across instruments (e.g., violin vs guitar vs flute)

## Tech Stack
- C# / .NET
- [NAudio](https://github.com/naudio/NAudio) — audio capture, playback, file I/O
- [MathNet.Numerics](https://numerics.mathdotnet.com/) — FFT and DSP math
- [ScottPlot](https://scottplot.net/) — waveform/spectrum/spectrogram plotting

## Role in the Umbrella Plan
This is the foundational project: its FFT/harmonic-extraction engine is intended
to be reused by `guitar-harmonic-fingerboard`, `harmonic-practice-assistant`, and
`physics-of-music`. See [`/plans/harmonics-projects-plan.md`](../plans/harmonics-projects-plan.md)
for the full rationale and project order.
