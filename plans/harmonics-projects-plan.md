# Musical Harmonics Projects — Selection & Repo Organization Plan

## Source
Ideas sourced from shared ChatGPT conversation "Software Project Ideas Harmonics"
(https://chatgpt.com/share/6a68c3c9-6ad8-83ea-904d-7be2fe1f3bc6), which proposed 15
harmonics-related software projects plus two larger concepts ("Harmonic Practice
Assistant" and "The Physics of Music").

## Selection Criteria (per user)
Prioritize projects related to: guitar, neuroscience/motor-rehab relevance, and the
"Physics of Music" umbrella concept — while keeping a sensible technical progression
(simple → advanced, shared groundwork first).

## Selected Projects (4), in build order

1. **`harmonic-spectrum-explorer/`** — *Idea #1, foundational*
   Load audio (file or mic), extract fundamental + harmonics via FFT, show
   waveform/spectrogram, play/mute/reconstruct individual harmonics.
   Rationale: lowest complexity, and its analysis engine (FFT, harmonic
   extraction) is the technical foundation the other guitar/neuro projects reuse.

2. **`guitar-harmonic-fingerboard/`** — *Idea #3, guitar-focused*
   Visualize natural/artificial harmonics on a guitar fretboard: nodes,
   antinodes, which fret produces which overtone, animated string vibration.
   Rationale: directly tied to user's guitar relearning interest; mostly
   visualization + music-theory logic, moderate complexity.

3. **`harmonic-practice-assistant/`** — *"Harmonic Practice Assistant" concept, guitar + neuroscience*
   Listens to practice (single note/chord), gives feedback on harmonic
   cleanliness, attack stability, unwanted overtones, and tracks progress over
   time (motor-rehab-style feedback loop).
   Rationale: the standout idea combining guitar technique + neuroscience/motor
   control interest; depends on the analysis engine from project 1 and
   fretboard/harmonic knowledge from project 2.

4. **`physics-of-music/`** — *"The Physics of Music" grand vision*
   Educational app combining modules: waves/interference, harmonic series,
   Fourier analysis, instrument timbre, guitar/piano harmonics, chords &
   consonance, tuning systems, resonance/standing waves, synthesis, spectral
   analysis.
   Rationale: largest scope; built last so it can reuse/reference the engines
   and lessons from projects 1–3 as modules rather than rebuilding from scratch.

## Tech Stack (confirmed)
C# / .NET, using:
- **NAudio** — audio capture/playback/file I/O
- **MathNet.Numerics** — FFT and DSP math
- **ScottPlot** — waveform/spectrum/spectrogram visualization

## Repo Organization
- New root folder **`plans/`** — holds this planning document
  (`plans/harmonics-projects-plan.md`) as the durable record of project
  selection/rationale, for future reference as work progresses.
- One root folder per selected project (sibling to `plans/`), each containing
  a `README.md` scaffold describing: goal, key features, tech stack, and
  status. No C# project files are scaffolded yet — that begins once a specific
  project is picked up for implementation.
- Root `README.md` updated with a short index linking to `plans/` and each
  project folder.

## Todos
- Create `plans/` folder with the planning document
- Scaffold `harmonic-spectrum-explorer/README.md`
- Scaffold `guitar-harmonic-fingerboard/README.md`
- Scaffold `harmonic-practice-assistant/README.md`
- Scaffold `physics-of-music/README.md`
- Update root `README.md` with links/index

## Notes
- Deliberately out of scope for this pass: the other 11 ideas from the chat
  (spectrum analyzer variants, ear trainer, room simulator, AI composer, etc.)
  — not selected because they don't match the guitar/neuroscience/Physics-of-Music
  focus. They remain documented in the source chat if reconsidered later.
- Actual C#/.NET solution scaffolding (csproj/sln, source code) is a follow-up
  step once one of these projects is picked for active implementation.
