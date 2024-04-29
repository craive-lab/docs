---
description: A set of frequently-asked questions about productions at the CRAIVE-Lab.
---

# FAQs

## Visual

<details>

<summary>If any of the projectors are not on, what should I do?</summary>

You can manually turn them on using remotes.

</details>

## Audio

<details>

<summary>How do I turn on the audio system if nothing is on?</summary>

Ideally, you should never worry about this, but in case it happens, here are the steps you should take in sequence to make sure the speakers are on:

* Check if the Opto-8 pre-amplifiers are on; if not, turn them on;
* Check if the Ferrofish control boxes are on; if not, turn them on;
* There are electrical switches behind the +X side of the visual display switches. The switches come in pairs. Turn on the switches one pair at a time.&#x20;

If hissy sounds come out of any of the speakers, turn everything above off in reverse order, and contact one of the [collaborators](contributing-to-the-craive-lab.md#researchers-at-the-craive-lab-and-rois-at-large).

</details>

<details>

<summary>What is vector-base amplitude panning?</summary>

Vector-base amplitude panning (VBAP) modulates the perceived loudness of spatially-positioned virtual sound sources based upon their distances to the listeners. Because it engages only limited amount of loudspeakers per virtual sound source, it is considered computationally efficient and is especially suited for real-time use. For this reason, it is also considered as the primary spatial audio rendering strategy at the CRAIVE-Lab. You can see it being used everywhere, from panoramic images to game-based applications.&#x20;

More useful information about VBAP can be found in [this textbook](https://link.springer.com/chapter/10.1007/978-3-030-17207-7\_3) (Zotter, 2019).

</details>

<details>

<summary>What is wave field synthesis?</summary>

Wave field synthesis (WFS) is one of the sound field rendering techniques that utilizes a physical boundary enclosed by a series of secondary sound sources (loudspeaker channels) to reconstruct sound fields based upon the spatial information of primary virtual sound sources, taking advantage of the Huygen-Fresnel principle. Although computationally more expensive than VBAP, it contributes to the enhancement of plausibility and congruency for the virtual environment immersed by the group occupants, and has extensive applications in spatial music compositions.

More useful information about WFS can be found in [this textbook](https://link.springer.com/book/10.1007/978-3-030-23033-3) (Ziemer, 2020).

</details>

<details>

<summary>What is Open Sound Control?</summary>



</details>

## Design

<details>

<summary>What is ROIS? What is the difference between ROIS and CAVE?</summary>

A room-oriented immersive system (ROIS) is a virtual reality system designed for in-person group interaction.&#x20;

</details>

<details>

<summary>The CRAIVE-Lab is capable of so many things! I want to produce my work with it but it overwhelms me. What is a good approach to start thinking about how my ideas can be realized?</summary>

You can start your design thinking based upon [a spatially-aware framework](https://www.sciencedirect.com/science/article/abs/pii/S000368702300114X?dgcid=author#preview-section-references) that we have created for ROIS (Huang et al., 2023).

Keep in mind, you do not have to utilize every single element. The framework is here to give you some clarity about how to best configure the spatial relationships that the CRAIVE-Lab produces in your production. Based upon the framework, your task is to decide what technologies to use within the CRAIVE-Lab, and what implementation strategies you adopt in your production to interface with them.

Also remember that this framework is not a be-all-end-all solution for your production, and it will evolve as more technologies are embedded into the CRAIVE-Lab and ROIS alike.

</details>
