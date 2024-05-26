# Project
- [Project](#project)
  - [Installing Stable Diffusion locally](#installing-stable-diffusion-locally)
    - [Installing homebrew](#installing-homebrew)
    - [Installing tools](#installing-tools)
    - [Cloning the AUTOMATIC1111 Web UI](#cloning-the-automatic1111-web-ui)
  - [Run Web UI](#run-web-ui)
  - [TouchDesigner with Stable Diffusion Tutorial](#touchdesigner-with-stable-diffusion-tutorial)
    - [Setting up TouchDesigner Project](#setting-up-touchdesigner-project)
    - [Adding music](#adding-music)
    - [Analying audio](#analying-audio)
    - [Creating the audio reactive visual](#creating-the-audio-reactive-visual)
      - [Create position and color of elements](#create-position-and-color-of-elements)
      - [Adding geometry](#adding-geometry)
      - [Adding geometry instances](#adding-geometry-instances)
        - [Positioning the instances](#positioning-the-instances)
        - [Adding color to the instances](#adding-color-to-the-instances)
        - [Adding rotation to the instances](#adding-rotation-to-the-instances)
        - [Adding animation](#adding-animation)
      - [Adding displacement](#adding-displacement)
      - [Adding noise](#adding-noise)
      - [Adding out node](#adding-out-node)
    - [Connecting audio reactive visual to stable diffusion](#connecting-audio-reactive-visual-to-stable-diffusion)
    - [Set up SD\_API](#set-up-sd_api)
    - [Set up prompt window](#set-up-prompt-window)
    - [Image generation settings](#image-generation-settings)
    - [Viewing the image in the background](#viewing-the-image-in-the-background)
    - [Adding feedback loop](#adding-feedback-loop)
    - [Adding logic to change frame when image is generated](#adding-logic-to-change-frame-when-image-is-generated)
    - [Adding frames](#adding-frames)
    - [Binding keep generating to record button](#binding-keep-generating-to-record-button)
    - [Start recording and generating images](#start-recording-and-generating-images)
    - [Using gpuhub for generation](#using-gpuhub-for-generation)
  - [Getting song information](#getting-song-information)
  - [Resources](#resources)
  - [Installing StreamDiffusion](#installing-streamdiffusion)
    - [Clone repo](#clone-repo)
    - [Create virtual environment](#create-virtual-environment)
  - [Timesyncing Lyrics](#timesyncing-lyrics)
  - [Prompt for keywords](#prompt-for-keywords)

## About this project
This project is part of the module computational perception extended by Guillaume Massol

## Goal
The goal of this project is to experiment with StableDiffusion and StreamDiffusion in Combination with TouchDesigner.

## Credits
This project was realized with various tool, techniques and content of third parties which are listed below:

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