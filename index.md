# Project
- [Project](#project)
  - [About this project](#about-this-project)
  - [Goal](#goal)
  - [Credits](#credits)
  - [Chapters](#chapters)
    - [Audio reactive visuals with TouchDesigner and Stable Diffusion web UI](#audio-reactive-visuals-with-touchdesigner-and-stable-diffusion-web-ui)
    - [Timelapse video of drawing with TouchDesigner and Stable Diffusion web UI](#timelapse-video-of-drawing-with-touchdesigner-and-stable-diffusion-web-ui)
    - [Music video with TouchDesigner and StreamDiffusion](#music-video-with-touchdesigner-and-streamdiffusion)

## About this project
This project is part of the module computational perception extended by Guillaume Massol

## Goal
The goal of this project is to experiment with StableDiffusion and StreamDiffusion in Combination with TouchDesigner.

## Credits
This project was realized with various tool, techniques and content of third parties which are listed below:
- [youtube.com - Marteria feat. ÄTNA & Yasha - Love, Peace & Happiness](https://www.youtube.com/watch?v=CsUQ0fEHGBE)
- [stability.ai - Stable Diffusion by StabilityAI](https://stability.ai/stable-image)
- [github.com - Stable Diffusion web UI by AUTOMATIC1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui/)
- [derivative.ca - Touch Designer by derivative](https://derivative.ca/)
- [github.com - Stream Diffusion](https://github.com/cumulo-autumn/StreamDiffusion)
- [patreon.com - Touch Designer Stable Diffusion and Stream Diffusion Components by dotsimulate](https://www.patreon.com/dotsimulate)
- [github.com - Touch Designer Lyrics Sync Component by GuiGPaP](https://github.com/GuiGPaP/TD_Lyrics)

## Chapters
### Audio reactive visuals with TouchDesigner and Stable Diffusion web UI
First, I worked with StableDiffusion web UI and TouchDesigner. I followed an extensive tutorial by [elekktronaut]() which introduced the workflow for creating visuals in TouchDesigner and then feeding it as img2img input to StableDiffusion web UI along with prompts to create audio reactive visuals.
The documentation of this part consists of various parts:
- [Stable Diffusion web UI installation](./stable-diffusion/stable-diffusion-install.md)
- [Floral diffusion tutorial documentation](./stable-diffusion/floral-diffusion/floraldiffusion.md)
- [Floral diffusion results](./stable-diffusion/floral-diffusion/index.md)

### Timelapse video of drawing with TouchDesigner and Stable Diffusion web UI
Second, I applied this workflow to create a timelapse video of a drawing of mine to use the timelapse of the drawing as input and extending it with Stable Diffusion web UI.
- [Head diffusion](./stable-diffusion/head-diffusion/index.md)

### Music video with TouchDesigner and StreamDiffusion
Third, I installed StreamDiffusion and created a music video for "Love, Peace and Happiness" with TouchDesigner in Combination with StreamDiffusion.
- [StreamDiffusion](./stream-diffusion/streamdiffusion.md)