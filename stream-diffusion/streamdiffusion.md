# StreamDiffusion

## Installing StreamDiffusion
An installation guide for StreamDiffusion is available on [github.com - StreamDiffusion](https://github.com/cumulo-autumn/StreamDiffusion).

By default, StreamDiffusion is not really developed with Mac in mind. Therefore, I did not follow the installation guide there.

In order to get StreamDiffusion running with TouchDesigner, there is a TouchDesigner Component by dotsimulate, which also provides easy installation.

![Stream Diffusion installation in TouchDesigner](./images/streamdiffusion-install.png)

Running it on Mac was not really straightforward. In order to get it running, I had to follow the installation, then create a virtual environment manually in the StreamDiffusion folder.

### Create virtual environment
```sh
python -m venv .venv
```

### Running StreamDiffusion from TouchDesigner component
The component also provided an easy way to run StreamDiffusion.
![Starting StreamDiffusion in TouchDesigner](./images/streamdiffusion-start.png)

At first, the integration only worked halfway, meaning I only got the first frame, then no updates. I did not fully solve this problem yet, however it seemed that the problem was gone, once I started the Stable Diffusion web UI before running StreamDiffusion.

### Feeding Noise into StreamDiffusion
To create an image with StreamDiffusion, we can use noise in combination with a prompt.

![TouchDesigner noise](./images/touchdesigner-noise.png)

In order to create an animation, the noise has to be animated which can be done by using `absTime.seconds`. In order to slow down the animation, this value can also be divided by a specific amount.

![Animating noise](./images/animating-noise.png)

### Creating the prompts
In order to have different prompts throughout the song, I wanted to timesync the prompt with the song. Luckily, someone already did the work to sync lyrics with a audiofile in operator: [github.com - TD_Lyrics](https://github.com/GuiGPaP/TD_Lyrics)

To get the timesynced lyrics, I had to do the manual work to correctly set the timestamps and create a .lrc file for the song.
> [Love, Peace & Happiness Lyrics](./lyrics/LovePeaceHappinessLyricsOnly.lrc)

#### Prompt for keywords
As a first step, I used Bing AI to create keywords, that describe the lyrics of the song. For this, I used the following prompt:
```
Here is a line of a song text: "Brauchst paar schnelle Nächte"
What could be descriptive keywords for image generation? Please only respond with a comma separated list of keywords
```

I executed this for every line of the song and then created a .lrc file from this which resulted in [Love, Peace & Happiness Keywords from Lyrics](./lyrics/LovePeaceHappinessKeywords.lrc)

TODO: add prompts, add results, add gifs