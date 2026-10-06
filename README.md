# Pix’n Portal Transfer Activity HUD

Experimental transfer activity indicator for Batocera/RGS.

The goal is simple: show when Pix’n Portal is actively downloading from or uploading to another user, so you know whether the system is safe to shut down.

## Current Behavior

```text
DOWN 9.60 Mbps
UP 35.8 Mbps
DOWN 9.60 Mbps   UP 35.8 Mbps
```

When no transfer is active, nothing is shown.

The monitor watches the RGS transfer log and tracks active P2P uploads/downloads. Transfer state is written to a small state file and can be displayed in-game through Batocera’s MangoHud integration.

## Current Status

- Real RGS download detection: working
- Real RGS upload detection: working
- Live speed updates: working
- In-game MangoHud display: working on tested titles
- Idle state: hidden
- Simultaneous upload/download display: supported
- EmulationStation/front-end display: still being worked on
- Some emulator/game launch paths still need compatibility testing

A real Pix’n Portal download was successfully displayed in-game as:

```text
DOWN 9.60 Mbps
```

This is still experimental and not ready for release yet.
