# Audio Amplifier PCB

This project is an audio amplifier PCB design that integrates a microphone input, auxiliary input, volume control, and an LM386 op-amp to amplify audio signals. The amplified signal can drive a speaker, with additional functionality to visually indicate signal strength using LEDs.

## Features

- **Microphone Input**: Captures audio via a condenser microphone and pre-amplifies it with a 2N3904 transistor.
- **Auxiliary Input**: Allows audio signals from external devices such as phones or MP3 players.
- **LM386 Op-Amp**: Used as the main amplifier, capable of delivering up to 36 dB of gain.
- **Volume Control**: Adjustable gain via a trimmer potentiometer and fine-tuned with a volume knob.
- **Visual Indicators**: Signal level displayed using LEDs of different colors (red, green, blue, yellow) driven by an LM339N comparator.
- **Speaker Output**: Amplified audio output to drive a connected speaker.
- **Auxiliary Out**: Allows amplified audio signals to be passed through a 3.5mm Jack.
## Schematic Overview

### Main Components
1. **Microphone Pre-Amp**:
   - A 2N3904 NPN transistor amplifies the microphone's signal.
   - Biasing resistors (R11, R12, R13) ensure proper operation.
   - Decoupling capacitors (C4, C5) filter noise from the signal.

2. **LM386 Amplifier**:
   - Amplifies the input signal (microphone or auxiliary) to drive the speaker.
   - Gain controlled via an adjustable resistor (Gain Adj, 4.7kΩ).
   - Decoupling and bypass capacitors (C6, C7, C10) ensure stable operation.

3. **Volume Control**:
   - A potentiometer (Volume Adj) allows the user to adjust the input signal level.

4. **LED Signal Indicators**:
   - An LM393N comparator drives LEDs to indicate signal levels.
   - Resistors (R1–R4) limit current through the LEDs.

5. **Power Supply**:
   - Powered by a 7-12V DC input (J2).
   - Decoupling capacitors (C1, C9) stabilize the power supply.

### Additional Features
- **Switches**:
  - SW1: Toggle between microphone and auxiliary input.
  - SW2: Power switch for the circuit.

- **Connectors**:
  - J1: Microphone/Auxiliary input.
  - J3: Speaker output.

## Applications

- DIY audio projects.
- Portable speaker systems.
- Signal visualization for audio signals.

## How to Use

1. Connect a microphone or auxiliary input to J1.
2. Adjust the volume using the potentiometer.
3. Connect a speaker to J3.
4. Power the circuit via J2 (7-12V DC).
5. Observe the LEDs for visual signal feedback.
