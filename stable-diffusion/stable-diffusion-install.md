# Installing Stable Diffusion locally
- [Installing Stable Diffusion locally](#installing-stable-diffusion-locally)
  - [Installing homebrew](#installing-homebrew)
  - [Installing tools](#installing-tools)
  - [Cloning the AUTOMATIC1111 Web UI](#cloning-the-automatic1111-web-ui)
  - [Run Web UI](#run-web-ui)


Taken from the guide at [stable-diffusion-art.com](https://stable-diffusion-art.com/install-mac/). Guide from AUTOMATIC1111 [github.com - Installation on Apple Silicon](https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Installation-on-Apple-Silicon)
## Installing homebrew
To install tools needed, we use homebrew, a package manager for macOS.
Installation can be found on [brew.sh](https://brew.sh/)

## Installing tools
There are some tools required to install first, these are python, wget and python:
```shell
brew install python@3.10 git wget
```

## Cloning the AUTOMATIC1111 Web UI
To get the Stable Diffusion WebUI, clone the git repository:
```shell
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui
```

## Run Web UI
The Web UI can be started after installing the tools and cloning the repo. Navigate to the repo and run the `webui.sh`:
```shell
cd stable-diffusion-webui
./webui.sh
```

This will take some time as it is also downloading some initial requirements.

After completing the startup, we should be able to access the Web UI on a local URL.