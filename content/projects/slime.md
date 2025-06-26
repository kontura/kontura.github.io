---
title: "Slime (C++, Compute shaders)"
---

{{< youtube LKzrWr1Vxvs >}}

<iframe id="odysee-iframe" style="width:100%; aspect-ratio:16 / 9;" src="https://odysee.com/%24/embed/%40SawMusic%3Ac%2FBroods-Peach_009%3A8?r=AapCoCa5Qc2Av5iQS4vDbjAsKVnP5gyE" allowfullscreen></iframe>

[Repository](https://github.com/kontura/slime)

This CLI program can generate visualisations based on sound (music) input.

It can work in an immediate mode where it uses the current system audio output. [PulseAudio](https://freedesktop.org/software/pulseaudio/doxygen/) API is used to get the data (Signed 16 Bit PCM).
Or an audio (.mp2) file can be provided directly which is read using [FFmpeg](http://ffmpeg.org/doxygen/6.0/).

Either way the data is then processed and used to generate next step in the slime simulation. The simulation is basically many individual agents whose behavior is a function of the audio input. Each agent moves around in the space a leaves a color trail on its path. The trail than disperses and evaporates over the next couple simulation steps.

I am also experimenting with other graphics. One is a more traditional spectrum analyser curve. Other current work in progress is a video of a fluid simulation.

Created video frames are shown on the screen and can be saved to a m4a video file (again using FFmpeg).
