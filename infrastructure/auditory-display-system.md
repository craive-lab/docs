---
description: >-
  This section provides an overview about the CRAIVE-Lab's auditory display
  system.
---

# Auditory Display System

## Basic Facts

<table><thead><tr><th width="296">Properties</th><th>Descriptions</th></tr></thead><tbody><tr><td>Total channel count</td><td>136 (128 for WFS, 6 for HoA, 2 for frontal stereo)</td></tr><tr><td>Rendering modalities</td><td>WFS + VBAP + HoA + Stereo</td></tr><tr><td>Max spatial aliasing frequency</td><td>603 Hz</td></tr><tr><td>Max virtual sound source count</td><td>256</td></tr></tbody></table>

## Speaker Map

<figure><img src="../.gitbook/assets/speaker_layout (1).png" alt=""><figcaption><p>Speaker map with their respected indexes in the infrastructure. Purple coordinates are compatible with game engines only.</p></figcaption></figure>

The speakers in the system represents 4 different kinds of rendering modalities:

* Vector-base amplitude panning (VBAP);
* Wave field synthesis (WFS);
* Higher-order ambisonics (HoA); and
* Stereo.

The correspondence between individual loudspeaker channels and their primary rendering modalities is listed below:

<table><thead><tr><th width="173" align="center">Channels</th><th align="center">Primary Rendering Modalities</th></tr></thead><tbody><tr><td align="center">1-128</td><td align="center">VBAP + WFS; certain channels assists in HoA rendering</td></tr><tr><td align="center">129-134</td><td align="center">HoA (assisted by certain channels in 1-128)</td></tr><tr><td align="center">135-136</td><td align="center">Stereo</td></tr></tbody></table>

The position and orientations of these loudspeakers affect the way virtual sound sources are rendered with respect to the physical space. You can find the exact coordinates with respect to the physical center of the room geometry in this CSV file (to be linked shortly).
