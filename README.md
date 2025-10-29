### Pocket Miku Web MIDI Controller

A browser-based controller for the Gakken NSX-39 “Pocket Miku” (Yamaha NSX-1 chip), built with Web MIDI. It provides a complete virtual instrument panel, including piano keys, performance wheels, MIDI CC sliders, and a Kaoss-style XY pad.

Features

Core MIDI Controls

Device/Channel Select – choose any available MIDI output; Ch.1 drives the eVocaloid engine, Ch.2–16 access GM/XG sounds.

Velocity & Octave – set default note velocity and transpose range.

Program Change – send GM/XG program numbers on channels 2–16.

Sustain, Mono/Poly Toggle – instant access to CC64 sustain and Omni modes.

CC Sliders

Quick access to important Control Change (CC) values:

CC1 – Modulation

CC7 – Volume

CC10 – Pan

CC11 – Expression

CC91 – Reverb Send

CC93 – Chorus Send

Piano & Wheels

On-screen Piano – two octaves of clickable/touchable keys.

QWERTY Keyboard Mapping – play notes using computer keys (Z–M, Q–U, etc.).

Pitch Bend & Mod Wheels – draggable/touch controls with spring-back pitch bend.

Harmony Helper

Adds an optional harmony note interval (±3rd, 5th, etc.) to every note played.

SysEx Tools

Directly send raw SysEx hex messages (e.g., NSX-1 lyric data).

Requires browser permission with sysex: true.

XY Pad (Kaoss-Style)

Drag/touch pad generates two CC streams simultaneously.

Assignable axes (X and Y) to any CC (1, 7, 10, 11, 71–74, 91, 93).

Toggle each axis independently.

Options to hold last values or reset to center/zero on release.

Thumb marker shows current position.

Usage

Serve the HTML file over HTTPS (Web MIDI requires a secure origin).

Click Connect MIDI (sysex) and allow access.

Select the Pocket Miku from the device list.

Use the piano, wheels, sliders, or XY pad to send MIDI data.

To send lyrics or advanced commands, enter raw SysEx hex bytes and press Send SysEx.

Notes for Pocket Miku

Channel 1 = eVocaloid voice synthesis. Requires SysEx to load lyric text.

Channels 2–16 = General MIDI / XG tone generator.

Some CCs (e.g., 71–74) adjust timbre, attack, brightness, etc., depending on voice.

Requirements

A modern browser with Web MIDI API (Chrome, Edge, Opera).

Secure origin (HTTPS or localhost).

Pocket Miku connected via USB-MIDI.

Future Ideas

Preset buttons for XY pad mappings.

Record/export MIDI performance.

Built-in lyric editor and SysEx sender for phoneme text.

License

MIT. Use and modify freely for fun Pocket Miku experiments.

Made by vUVu

https://github.com/vuvuvu/pocket-miku-midi

