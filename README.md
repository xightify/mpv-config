<h1 align="center">- mpv-config -</h1>
<h3 align="center"><samp>my personal mpv config files</samp></h3>

<img width="2560" height="1440" alt="showcase000" src="https://github.com/user-attachments/assets/fd1b8290-2b73-470f-8d2f-14405388c5f0" />

<img width="2560" height="1440" alt="showcase001" src="https://github.com/user-attachments/assets/54c54c01-0e2f-4514-9977-e54b89de7c34" />

<img width="2560" height="1440" alt="showcase002" src="https://github.com/user-attachments/assets/b18dabf3-4e2c-4607-8534-7584a2a3f198" />

<img width="2560" height="1440" alt="showcase003" src="https://github.com/user-attachments/assets/50d1f9f3-de72-4cde-997c-751ffe9a4d16" />

<img width="2560" height="1440" alt="showcase004" src="https://github.com/user-attachments/assets/ba7deb73-ac5b-49e4-a839-32205f430ccf" />


## Requirements

- mpv  
- ffmpeg  
- yt-dlp  

## Installation:
- **Windows:**
	- https://github.com/shinchiro/mpv-winbuild-cmake/releases  
	- https://github.com/zhongfly/mpv-winbuild/releases  
- **macOS:**
	- `brew install mpv`
- **Linux:**
	- Fedora
		- `sudo dnf install mpv`
	- Arch Linux / Manjaro
		- `sudo pacman -S mpv`
	- Ubuntu / Debian-based
		- `sudo apt update && sudo apt install mpv`

## Download Tips for Windows:
- 64 bit - mpv-x86_64-YYYYMMDD-git - for maximum compatibility
- 64 bit - mpv-x86_64-v3-YYYYMMDD-git - recommended for most modern systems (Intel Haswell 2013+, AMD Zen+)
- ARM64 - mpv-aarch64-YYYYMMDD-git - for Windows on ARM devices

## Setup

1. Extract mpv-x86_64-v3-YYYYMMDD-git.7z
2. Rename folder to `mpv`  
3. Move `mpv` to
    -   **Windows:**
		- **Option I:** 
			- `C:\Users\%Username%\AppData\Roaming\mpv`
		- **Option II:** 
			- Move `mpv` anywhere you like
4. Run `mpv-install.bat` or `register.bat` (for file associations)

- 	**Linux and macOS:** `~/.config/mpv`

## Folder Structure

    mpv/
    │   ffmpeg.exe
    │   mpv.exe
    │   updater.bat
    │   yt-dlp.exe
    │
    └── portable_config/
        │   input.conf
        │   mpv.conf
        │   watch_history.jsonl
        │   profiles.conf
        │
        ├── cache/
        │   ├── shaders_cache
        │   └── watch_later
        │
        ├── fonts/
        │   └── ryo-icons.ttf
        │
        ├── script-opts/
        │   ├── anilist_rpc.conf
        │   ├── media_rpc.conf
        │   ├── ryo-osc.conf
        │   ├── deband-cycle.conf
        │   ├── subtitle.conf
        │   ├── console.conf
        │   └── stats.conf
        │
        ├── scripts/
        │   ├── anilist_rpc.lua
        │   ├── media_rpc.lua
        │   ├── ryo-osc.lua
		│	├── lang-seek.lua
        │   ├── deband-cycle.lua
        │   ├── subtitle.lua
        │   ├── thumbfast.lua
        │   ├── evafast.lua
        │   ├── silentskip.lua
        │   └── webm.lua
        │
        └── shaders/
            └── .glsl files


## Scripts
- **[ryo-osc](https://github.com/Xightify/ryo-osc)** - My personal OSC fork based on **[hayase-osc](https://github.com/nekoxuee/hayase-osc)**.
- **deband-cycle, anilist_rpc, media_rpc, subtitle, lang-seek** are all made by me.
- **[evafast](https://github.com/po5/evafast)** - Fast-forwarding and seeking on a single key, with quality of life features like a slight slowdown when subtitles are shown.
- **[silentskip](https://github.com/nekoxuee/mpv-config/blob/main/scripts/silentskip.lua)** - Skip intros/endings manually, with silence-detection fallback.
- **[thumbfast](https://github.com/po5/thumbfast)** - High-performance on-the-fly thumbnailer script for mpv.
- **[webm](https://github.com/ekisu/mpv-webm)** - Quickly create video clips.

## Shaders
- **[AniSD ArtCNN](https://github.com/Sirosky/Upscale-Hub/releases/tag/AniSD-ArtCNN)**
- **[Ani4K v2 ArtCNN](https://github.com/Sirosky/Upscale-Hub/releases/tag/Ani4k-v2-ArtCNN)**
- **[ArtCNN](https://github.com/Artoriuz/ArtCNN)**
- **[CfL_Prediction](https://github.com/Artoriuz/glsl-chroma-from-luma-prediction)**
- **[Anime4k](https://github.com/bloc97/Anime4K)**

## Fonts
- Gandhi Sans  
- Century Gothic Bold
- Netflix Sans Bold
- Gabarito Regular
- JetBrainsMono Regular

## Tested Hardware

- Desktop: Ryzen 9 9950X3D, RTX 5080, 64 GB DDR5, Windows 11 Pro
- Laptop: Core i7-12700H, RTX 3070, 32 GB DDR5, Windows 11 Pro, Fedora

## Fix NVIDIA Overlay Issue

Alt + Z → Settings → Notifications → Disable "Open/close in-game overlay"

## References
- **[iamscum](https://iamscum.wordpress.com/guides/videoplayback-guide/mpv-conf/)**
- **[mpv manual](https://mpv.io/manual/stable/)**

## Other Configs
- https://github.com/nekoxuee/mpv-config
- https://github.com/Zabooby/mpv-config/
- https://github.com/tuilakhanh/mpv-config/
- https://github.com/itsmeipg/mpv-config/
- https://github.com/noelsimbolon/mpv-config/
- https://github.com/HongYue1/mpv-config
