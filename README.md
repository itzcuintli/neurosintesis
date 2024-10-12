# Audio Generation from EEG Data

1. **Data Source**: This project utilizes data from a Muse 2 EEG device, with myself as the test subject :D

2. **Delta Waves**: The code processes EEG data with a focus on delta waves, which are low-frequency brain waves typically ranging from 0.5 to 4 Hz. These waves are most prominent during deep sleep and restorative states, playing a crucial role in healing and regeneration. They are also associated with deep, dreamless sleep and meditative states.

3. **Functionality**: The code takes the EEG data and produces a visual plot of the data, three distinct audio outputs (each lasting 30 seconds), and spectrograms for analysis.

## 1. Synth Audio (Synth-Pulse)

### Adjustments for Synth Audio
- **Map Frequencies to Musical Scale**: Frequencies derived from EEG data are mapped to the C Major scale.
- **Harmonic Progression**: The audio incorporates a carefully arranged sequence of notes that rise and fall, creating a sense of movement within the sound.

### Key Features Explained
- **Harmonic Frequency Range**: Frequencies correspond to notes in the C Major scale, providing a clear and consonant sound.
- **Sine Wave Waveform**: Utilizes a pure sine wave, resulting in smooth, clean tones that resonate clearly.

## 2. Dynamically Mapped Audio (Mapped Wave)

### Adjustments for Dynamically Mapped Audio
- **Segmented Construction**: The audio is generated in segments, allowing for varying pitches and layered sounds that evolve throughout the piece.
- **Dynamic Volume Adjustments**: Each segment’s volume is influenced by the EEG-derived volume factor, resulting in noticeable shifts in intensity.

### Key Features Explained
- **Complex Waveform**: Combines multiple sine waves across segments, creating a rich auditory texture.
- **Unique Frequency Signature**: Frequencies are directly derived from the EEG data, leading to a distinctive sound profile.

## 3. ECG-Like Heart Sound (ECG-Heartbeat)

### Adjustments for ECG-like Heart Sound
- **Create a Pulsating Effect**: Uses a square wave to simulate the sharp peaks of a heartbeat.
- **Modify Frequency and Volume Dynamically**: Adjusts volume to create a realistic "thump" effect, mimicking a heartbeat's rhythm.

### Key Features Explained
- **Lower Frequency**: The base frequency is set lower (multiplied by 0.6) to simulate a deeper heartbeat sound.
- **Square Wave Pulse**: Generates distinct "thump" sounds, with a pulse frequency set to 1 Hz to represent a heartbeat (60 BPM).
- **Combining Waveforms**: Merges the pulse with the sine wave to enhance rhythmic depth.

## Next Steps
- **Producing an Ableton Plugin**: The next step involves creating a Max for Live device in Ableton that integrates this audio generation process, allowing for real-time control and visualization of EEG-derived sounds.