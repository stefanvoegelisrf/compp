# Project
- [Project](#project)
  - [About this project](#about-this-project)
  - [Goal](#goal)
  - [Credits](#credits)
  - [Chapters](#chapters)
    - [Audio reactive visuals with TouchDesigner and Stable Diffusion web UI](#audio-reactive-visuals-with-touchdesigner-and-stable-diffusion-web-ui)
    - [Timelapse video of drawing with TouchDesigner and Stable Diffusion web UI](#timelapse-video-of-drawing-with-touchdesigner-and-stable-diffusion-web-ui)
    - [Music video with TouchDesigner and StreamDiffusion](#music-video-with-touchdesigner-and-streamdiffusion)
  - [Reflection](#reflection)
  - [Resources](#resources)

## About this project
This project is part of the module computational perception extended by Guillaume Massol

## Goal
The goal of this project is to experiment with StableDiffusion and StreamDiffusion in Combination with TouchDesigner.
In this project I wanted to explore the realtime possibilites with Image Generation in Combination with Music. I also wanted to get to know several workflows which I can take up in the future to create AI generated visuals. I limited myself to my personal Hardware which was a Macbook Pro with M2 Max. Inititally, my goal was to create several audio reactive visuals which are based on Lyrics of the song "Love, Peace and Happiness" by Marteria and then feed these Visuals into StableDiffusion or StreamDiffusion. This scope was too big and I scaled it down to creating an animation with prompts only. In the future i want to take this up again and create further animations with the techniques I learned in this project.

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

## Reflection
I was able to get several workflows running and was able to create multiple animations. Initially, my scope was too big, but I adjusted it and focused on the workflows with TouchDesigner, StableDiffusion and StreamDiffusion.


My first experiment, where I mainly followed a tutorial by elekktronaut, gave me a very good look into how I can approach the workflow with creating visuals in TouchDesigner and taking these visuals as an input for Image Generation. The amount of time that I have to spend for creating these visuals is quite large, which I underestimated quite a bit. For future projects, I would plan more time, have a smaller scope and also plan the visuals out in detail. The amount of time it takes to create an image with the TouchDesigner-StableDiffusion workflow was about 14 seconds an image on my Mac. For a whole music video, this is a very large amount and for future projects, I would use better hardware or optimize the image generation process as much as possible.
An important part of this workflow is, that the generated images are also used an input for image generation, to generate images that resemble each other so the transitions between images are not hard.


In my second experiment, I applied the first workflow onto my personal drawings, to figure out what I can make of a timelapse drawing with image generation. I learned a lot about how the settings in StableDiffusion matter for the image generation, in my case mainly the denoising strength, the noise multiplier and also the step count. These settings are still a bit confusing to me and I want to learn more about them to get to know the meaning of them better. I only scratched the surface and in the future would also use controlnet, LoRAs and more advanced techniques. I will also take this up later on and create more timelapse animations.


In my third experiment, I struggled a bit to even get it running. This was quite frustrating, but to be expected as my hardware was not optimal to try this out. I should have tried to get access to a machine that was more suite. Luckily, I was not the only person with a Mac that wants to try this workflow, so in the last weeks of the project, other people figured out to get it running.
Timesyncing prompts to my audio would have been a pain to implement, if it weren't for other work that already figured this out. My knowledge is a bit too basic at this point to do this in TouchDesigner, even though my programming knowledge is strong. This showed me that I need to dive into TouchDesigner more and get better at it. At some point I also realized, that I won't be able to create visuals as input, which is why I focussed on getting fitting prompts for the song lyrics and only use noise as image generation input. The results look nice, but I learned that for another project like this, I should plan out the visuals much more in detail and also abstract the visuals. Just trying to visualize the lyrics is not enough. In the future I also want to try out more image generation models to see which one fits best and I also want to get better at prompting. With my Mac, I got a low framerate, which is why I would also opt for a better machine in the future. Nevertheless, I am satisfied with my results, as I got the technical setup running and got appealing visual outputs for the lyrics and also learned more about prompting and how I can set up a project like this.


## Resources
- [stable-diffusion-art.com - How Stable Diffusion works](https://stable-diffusion-art.com/how-stable-diffusion-work/)
- [imaginewithrashid.com - AI image generation art styles](https://imaginewithrashid.com/different-art-styles-for-ai-image-generation/)
- [kdnuggets.com - Realistic Faces with Stable Diffusion](https://www.kdnuggets.com/3-ways-to-generate-hyper-realistic-faces-using-stable-diffusion)
- [colab.research.google.com](https://colab.research.google.com/)
- [tensorflow.org](https://www.tensorflow.org/js#getting-started)
- [mlart.co](https://mlart.co/)
- [github.com - Foocus](https://github.com/lllyasviel/Fooocus)
- [github.com - Stable Diffusion web UI](https://github.com/AUTOMATIC1111/stable-diffusion-webui/)
- [github.com - Stream Diffusion](https://github.com/cumulo-autumn/StreamDiffusion)
- [patreon.com - dotsimulate](https://www.patreon.com/dotsimulate/)
- [elekktronaut.com](https://www.elekktronaut.com/)
- [confusedbit.dev - How does GPT work](https://confusedbit.dev/posts/how_does_gpt_work/)
- [youtube.com - Google Cloud Tech - Transformers, explained: Understand the model behind GPT, BERT, and T5](https://www.youtube.com/watch?v=SZorAJ4I-sA)
- [youtube.com - ByteByteGo - How ChatGPT Works Technically - ChatGPT Architecture](https://www.youtube.com/watch?v=bSvTVREwSNw)