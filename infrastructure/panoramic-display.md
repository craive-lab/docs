---
description: >-
  This section provides an overview about the CRAIVE-Lab's visual display
  system.
---

# Panoramic Display

{% hint style="danger" %}
**Please do not touch the projection screen!** The screen material is a type of micro-perforated fabric that is vulnerable to physical impact. Please exercise restraints when designing physical interactions in close proximity to its surface.&#x20;
{% endhint %}

## Basic Facts

<table><thead><tr><th width="219">Properties</th><th>Descriptions</th></tr></thead><tbody><tr><td>Spatial Footprint (m)</td><td>W10 x L12 x H4.264; Corner: 1.518m filleted radius.</td></tr><tr><td>Display Resolution</td><td>15360 x 1200 (12.8:1)</td></tr><tr><td>Production Resolution</td><td>11636 x 1200 (9.7:1)</td></tr><tr><td>Projector Count</td><td>8</td></tr><tr><td>Field of View</td><td>Horizontal FoV 346.6°; Vertical FoV: 39.0° - 45.9°. </td></tr></tbody></table>

{% hint style="info" %}
**What is the difference between production resolution and display resolution?**

Production resolution is the resolution without distortions on a standard computer monitor. This resolution is distorted on the CRAIVE-Lab's panoramic display.&#x20;

Display resolution is the resolution that is undistorted on the CRAIVE-Lab's panoramic display. It looks stretched on a standard computer monitor.

See [Panoramas](panoramic-display.md#panoramas) and [Display panoramas from spherical cameras](../examples/4.-display-panorama-from-spherical-camera.md) for more detail.
{% endhint %}

## Pixel-Perfect Dimensional Marker of Visual Display

<figure><img src="../.gitbook/assets/dimensions.png" alt=""><figcaption><p>Pixel dimensions of each critical display boundary in the physical space. The display is unwrapped. Click on the image to expand.</p></figcaption></figure>

{% hint style="info" %}
A numerical version of all the key pixel coordinates, along with their corresponding stretched coordinates, physical and pixel dimensions, proportions, and angular coordinates, can be found in [this Google Sheet document](https://docs.google.com/spreadsheets/d/13L-cFcvPIDc2OT34PLLkPOo-239FWXvqXio3jRufNsQ/edit?usp=sharing).
{% endhint %}

## Panoramas&#x20;

<figure><img src="../.gitbook/assets/panorama.png" alt=""><figcaption><p>Compensation stretching of panoramic image for correct perspective in panoramic display. Click on the image to expand.</p></figcaption></figure>

The CRAIVE-Lab's continuous 360° projection is made up of 8 projectors. The permanent display is not quite 360° due to the gap present in the entrance, but can be made so by adding temporary drapery. Each projector has an aspect ratio of 16:10 and a pixel resolution of `1920x1200`. However, to achieve a single, seamless projection, the projections from each projectors are overlapped and blended together. So even though the combined native resolution of all eight projectors is `15360x1200` (`1920x8=15360`), those 15,360 horizontal pixels are being “squeezed” into a narrower screen space in order to allow for the smooth blending between overlapped projectors. In other words, instead of the expected `128:10` aspect ratio, the same resolution is squeezed into an aspect ratio of `97:10`.&#x20;

What this means for content creators is that a `15360 x 1200` pixel image which looks fine on your screen would look “squeezed” or “skinny” when displayed at the CRAIVE-Lab.&#x20;

To offset this intrinsic squeezing distortion, the very last thing you should do before completing any imagery for the CRAIVE-Lab – whether from photography, line work, renderings, animations, etc. – is add a “pre-squeeze” compensation. This will consist of a simple stretching distortion to “fatten” your imagery so that when it is projected in CRAIVE it looks as you intend.&#x20;

{% hint style="info" %}
There is one exception to this: real-time interactive contents. Dynamic cameras can be set up so that distortion adjustments is generally not needed. However, this does not necessarily mean that the perspective distortion is automatically corrected. The exact mechanism of such correction for real-time environments is currently a research topic.
{% endhint %}

**Please note**: the final image which is ready for CRAIVE will look distorted (“fat”) on your screen, which is correct!&#x20;

The simplest workflow is to use a canvas size of `11636 x 1200`, lay out your content referencing the guides shown here (at right), and at the very end when the image is done, change the canvas size to `15360 x 1200` – in other words, stretch everything horizontally by `132%`. It will look “fat” on your screen, but normal at the CRAIVE-Lab.

### Rendering 3D Assets

See [Create panoramic renders using V-Ray](../examples/5.-rendering-panorama.md) for more detail.

## Field of View

<figure><img src="../.gitbook/assets/fovs.png" alt=""><figcaption><p>Diagram indicating horizontal and vertical fields of view. Purple indicators are for game engines only. Click on image to expand.</p></figcaption></figure>

The CRAIVE screen is quite large, but still only fills a fraction of the field of view of someone’s 360° sphere of vision.&#x20;

The horizontal field of view (hFOV) for a viewer standing in the center of the screen area and facing the short wall opposite the entrance has a total hFOV = 346.6° (196.5° turning the head to the left and 150.1° toward the right).&#x20;

The vertical field of view (vFOV) varies since the screen does not conform to a cylindrical or spherical shape, but rather follows a rounded rectangle, which changes the angles to the top and bottom edges around the screen.&#x20;

When facing the short walls from the middle of the screen area, the vFOV = 39.0° (15.4° below and 23.6° above an average eye height of 5’ 5”).&#x20;

When facing the long walls, which are slightly closer to the viewer, the vFOV = 45.9° (18.3° below and 27.6° above an average eye height of 5’ 5”).&#x20;

For content creators working with virtual models, you can set the point of view (POV) location and then create guides emanating from the POV eye height in order to see what in the distance will fall within CRAIVE’s vFOV. But keep in mind that the vFOV becomes less as you look away from the centers of the flat walls (since the screen is effectively shrinking as it gets further away from the viewer), so plan accordingly.&#x20;

When generating equirectangular imagery (see next page), use the “CRAIVE screen bounds.png” as an overlay on your image to get a sense of what will fall within the vFOV around the screen.

### Dynamic Rendering

See [Unity](../software/unity.md) and [Unreal Engine + Twinmotion](../software/unreal-engine-coming-soon.md).

## Distortion Adjustments&#x20;

Specialized tools are available for distortion adjustments. Please contact us for more information (This part to be edited by Sam).

##
