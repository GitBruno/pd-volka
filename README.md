# PD - Volka

**PD patches targeting the Korg Volka range.**

Mainly exist of MIDI generators but also a place where to save some collected docs.

## Volka Global Settings

Get into the global menu by holding `FUNC` when powering on.

| Step | Control                | Notes                                 |
|-----:|:-----------------------|:--------------------------------------|
| 1    | auto-power-off         | on/off                                |
| 2    | battery type           | nH (rechargeable) or AL (alkaline)    |
| 3    | polarity sync out      | Low / High                            |
| 4    | polarity sync in       | Low / High                            |
| 5    | bpm range              | nR (Narrow: 60–240) FR (Full: 10–600) |
| 6    | MIDI clock             | Au (Auto) / In (Ignore)               |
| 7    | MIDI RX ShortMessage   | on/off                                |
| 8    | Sync input/output unit | Once a step / Once every 2 steps      |

## Volka Sample MIDI CC

Control messages for Parts 1 – 10 (Channel 1 – 10):*

| MIDI CC | Control                | Notes                      |
|--------:|:-----------------------|:---------------------------|
| 7       | LEVEL                  |                            |
| 10      | PAN                    |                            |
| 40      | SAMPLE START POINT     |                            |
| 41      | SAMPLE LENGTH          |                            |
| 42      | HI CUT                 |                            |
| 43      | SPEED                  | Values 0–127 map to -63–63 |
| 44      | PITCH EG INT           | Values 0–127 map to -63–63 |
| 45      | PITCH EG ATTACK        |                            |
| 46      | PITCH EG DECAY         |                            |
| 47      | AMP EG ATTACK          |                            |
| 48      | AMP EG DECAY           |                            |

## Volka FM MIDI CC

Received when global parameter MIDI RX ShortMessage is set to ON.

| MIDI CC | Control          | Notes |
|--------:|:-----------------|:------|
| 40      | TRANSPOSE        |       |
| 41      | VELOCITY         |       |
| 42      | MODULATOR ATTACK |       |
| 43      | MODULATOR DECAY  |       |
| 44      | CARRIER ATTACK   |       |
| 45      | CARRIER DECAY    |       |
| 46      | LFO RATE         |       |
| 47      | LFO PITCH DEPTH  |       |
| 48      | ALGORITHM        |       |
| 49      | ARP TYPE         |       |
| 50      | ARP DIV          |       |

