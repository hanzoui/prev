<div align="center">

# Hanzo Studio
**The most powerful and modular visual AI engine and application.**


[![Website][website-shield]][website-url]
[![Dynamic JSON Badge][discord-shield]][discord-url]
[![Twitter][twitter-shield]][twitter-url]
[![Matrix][matrix-shield]][matrix-url]
<br>
[![][github-release-shield]][github-release-link]
[![][github-release-date-shield]][github-release-link]
[![][github-downloads-shield]][github-downloads-link]
[![][github-downloads-latest-shield]][github-downloads-link]

[matrix-shield]: https://img.shields.io/badge/Matrix-000000?style=flat&logo=matrix&logoColor=white
[matrix-url]: https://app.element.io/#/room/%23hanzo_studio_space%3Amatrix.org
[website-shield]: https://img.shields.io/badge/ComfyOrg-4285F4?style=flat
[website-url]: https://hanzo.ai/
<!-- Workaround to display total user from https://github.com/badges/shields/issues/4500#issuecomment-2060079995 -->
[discord-shield]: https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fdiscord.com%2Fapi%2Finvites%2Fcomfyorg%3Fwith_counts%3Dtrue&query=%24.approximate_member_count&logo=discord&logoColor=white&label=Discord&color=green&suffix=%20total
[discord-url]: https://hanzo.ai/discord
[twitter-shield]: https://img.shields.io/twitter/follow/Hanzo Studio
[twitter-url]: https://x.com/Hanzo Studio

[github-release-shield]: https://img.shields.io/github/v/release/hanzoai/studio?style=flat&sort=semver
[github-release-link]: https://github.com/hanzoai/studio/releases
[github-release-date-shield]: https://img.shields.io/github/release-date/hanzoai/studio?style=flat
[github-downloads-shield]: https://img.shields.io/github/downloads/hanzoai/studio/total?style=flat
[github-downloads-latest-shield]: https://img.shields.io/github/downloads/hanzoai/studio/latest/total?style=flat&label=downloads%40latest
[github-downloads-link]: https://github.com/hanzoai/studio/releases

![Hanzo Studio Screenshot](https://github.com/user-attachments/assets/7ccaf2c1-9b72-41ae-9a89-5688c94b7abe)
</div>

Hanzo Studio lets you design and execute advanced stable diffusion pipelines using a graph/nodes/flowchart based interface. Available on Windows, Linux, and macOS.

## Get Started

#### [Desktop Application](https://hanzo.ai/download)
- The easiest way to get started.
- Available on Windows & macOS.

#### [Windows Portable Package](#installing)
- Get the latest commits and completely portable.
- Available on Windows.

#### [Manual Install](#manual-install-windows-linux)
Supports all operating systems and GPU types (NVIDIA, AMD, Intel, Apple Silicon, Ascend).

## [Examples](https://hanzoai.github.io/HanzoStudio_examples/)
See what Hanzo Studio can do with the [example workflows](https://hanzoai.github.io/HanzoStudio_examples/).

## Features
- Nodes/graph/flowchart interface to experiment and create complex Stable Diffusion workflows without needing to code anything.
- Image Models
   - SD1.x, SD2.x ([unCLIP](https://hanzoai.github.io/HanzoStudio_examples/unclip/))
   - [SDXL](https://hanzoai.github.io/HanzoStudio_examples/sdxl/), [SDXL Turbo](https://hanzoai.github.io/HanzoStudio_examples/sdturbo/)
   - [Stable Cascade](https://hanzoai.github.io/HanzoStudio_examples/stable_cascade/)
   - [SD3 and SD3.5](https://hanzoai.github.io/HanzoStudio_examples/sd3/)
   - Pixart Alpha and Sigma
   - [AuraFlow](https://hanzoai.github.io/HanzoStudio_examples/aura_flow/)
   - [HunyuanDiT](https://hanzoai.github.io/HanzoStudio_examples/hunyuan_dit/)
   - [Flux](https://hanzoai.github.io/HanzoStudio_examples/flux/)
   - [Lumina Image 2.0](https://hanzoai.github.io/HanzoStudio_examples/lumina2/)
   - [HiDream](https://hanzoai.github.io/HanzoStudio_examples/hidream/)
   - [Qwen Image](https://hanzoai.github.io/HanzoStudio_examples/qwen_image/)
   - [Hunyuan Image 2.1](https://hanzoai.github.io/HanzoStudio_examples/hunyuan_image/)
   - [Flux 2](https://hanzoai.github.io/HanzoStudio_examples/flux2/)
   - [Z Image](https://hanzoai.github.io/HanzoStudio_examples/z_image/)
- Image Editing Models
   - [Omnigen 2](https://hanzoai.github.io/HanzoStudio_examples/omnigen/)
   - [Flux Kontext](https://hanzoai.github.io/HanzoStudio_examples/flux/#flux-kontext-image-editing-model)
   - [HiDream E1.1](https://hanzoai.github.io/HanzoStudio_examples/hidream/#hidream-e11)
   - [Qwen Image Edit](https://hanzoai.github.io/HanzoStudio_examples/qwen_image/#edit-model)
- Video Models
   - [Stable Video Diffusion](https://hanzoai.github.io/HanzoStudio_examples/video/)
   - [Mochi](https://hanzoai.github.io/HanzoStudio_examples/mochi/)
   - [LTX-Video](https://hanzoai.github.io/HanzoStudio_examples/ltxv/)
   - [Hunyuan Video](https://hanzoai.github.io/HanzoStudio_examples/hunyuan_video/)
   - [Wan 2.1](https://hanzoai.github.io/HanzoStudio_examples/wan/)
   - [Wan 2.2](https://hanzoai.github.io/HanzoStudio_examples/wan22/)
   - [Hunyuan Video 1.5](https://docs.hanzo.ai/tutorials/video/hunyuan/hunyuan-video-1-5)
- Audio Models
   - [Stable Audio](https://hanzoai.github.io/HanzoStudio_examples/audio/)
   - [ACE Step](https://hanzoai.github.io/HanzoStudio_examples/audio/)
- 3D Models
   - [Hunyuan3D 2.0](https://docs.hanzo.ai/tutorials/3d/hunyuan3D-2)
- Asynchronous Queue system
- Many optimizations: Only re-executes the parts of the workflow that changes between executions.
- Smart memory management: can automatically run large models on GPUs with as low as 1GB vram with smart offloading.
- Works even if you don't have a GPU with: ```--cpu``` (slow)
- Can load ckpt and safetensors: All in one checkpoints or standalone diffusion models, VAEs and CLIP models.
- Safe loading of ckpt, pt, pth, etc.. files.
- Embeddings/Textual inversion
- [Loras (regular, locon and loha)](https://hanzoai.github.io/HanzoStudio_examples/lora/)
- [Hypernetworks](https://hanzoai.github.io/HanzoStudio_examples/hypernetworks/)
- Loading full workflows (with seeds) from generated PNG, WebP and FLAC files.
- Saving/Loading workflows as Json files.
- Nodes interface can be used to create complex workflows like one for [Hires fix](https://hanzoai.github.io/HanzoStudio_examples/2_pass_txt2img/) or much more advanced ones.
- [Area Composition](https://hanzoai.github.io/HanzoStudio_examples/area_composition/)
- [Inpainting](https://hanzoai.github.io/HanzoStudio_examples/inpaint/) with both regular and inpainting models.
- [ControlNet and T2I-Adapter](https://hanzoai.github.io/HanzoStudio_examples/controlnet/)
- [Upscale Models (ESRGAN, ESRGAN variants, SwinIR, Swin2SR, etc...)](https://hanzoai.github.io/HanzoStudio_examples/upscale_models/)
- [GLIGEN](https://hanzoai.github.io/HanzoStudio_examples/gligen/)
- [Model Merging](https://hanzoai.github.io/HanzoStudio_examples/model_merging/)
- [LCM models and Loras](https://hanzoai.github.io/HanzoStudio_examples/lcm/)
- Latent previews with [TAESD](#how-to-show-high-quality-previews)
- Works fully offline: core will never download anything unless you want to.
- Optional API nodes to use paid models from external providers through the online [Comfy API](https://docs.hanzo.ai/tutorials/api-nodes/overview).
- [Config file](extra_model_paths.yaml.example) to set the search paths for models.

Workflow examples can be found on the [Examples page](https://hanzoai.github.io/HanzoStudio_examples/)

## Release Process

Hanzo Studio follows a weekly release cycle targeting Monday but this regularly changes because of model releases or large changes to the codebase. There are three interconnected repositories:

1. **[Hanzo Studio Core](https://github.com/hanzoai/studio)**
   - Releases a new stable version (e.g., v0.7.0) roughly every week.
   - Starting from v0.4.0 patch versions will be used for fixes backported onto the current stable release.
   - Minor versions will be used for releases off the master branch.
   - Patch versions may still be used for releases on the master branch in cases where a backport would not make sense.
   - Commits outside of the stable release tags may be very unstable and break many custom nodes.
   - Serves as the foundation for the desktop release

2. **[Hanzo Desktop](https://github.com/hanzoui/desktop)**
   - Builds a new release using the latest stable core version

3. **[Hanzo Frontend](https://github.com/hanzoui/studio_frontend)**
   - Weekly frontend updates are merged into the core repository
   - Features are frozen for the upcoming core release
   - Development continues for the next release cycle

## Shortcuts

| Keybind                            | Explanation                                                                                                        |
|------------------------------------|--------------------------------------------------------------------------------------------------------------------|
| `Ctrl` + `Enter`                      | Queue up current graph for generation                                                                              |
| `Ctrl` + `Shift` + `Enter`              | Queue up current graph as first for generation                                                                     |
| `Ctrl` + `Alt` + `Enter`                | Cancel current generation                                                                                          |
| `Ctrl` + `Z`/`Ctrl` + `Y`                 | Undo/Redo                                                                                                          |
| `Ctrl` + `S`                          | Save workflow                                                                                                      |
| `Ctrl` + `O`                          | Load workflow                                                                                                      |
| `Ctrl` + `A`                          | Select all nodes                                                                                                   |
| `Alt `+ `C`                           | Collapse/uncollapse selected nodes                                                                                 |
| `Ctrl` + `M`                          | Mute/unmute selected nodes                                                                                         |
| `Ctrl` + `B`                           | Bypass selected nodes (acts like the node was removed from the graph and the wires reconnected through)            |
| `Delete`/`Backspace`                   | Delete selected nodes                                                                                              |
| `Ctrl` + `Backspace`                   | Delete the current graph                                                                                           |
| `Space`                              | Move the canvas around when held and moving the cursor                                                             |
| `Ctrl`/`Shift` + `Click`                 | Add clicked node to selection                                                                                      |
| `Ctrl` + `C`/`Ctrl` + `V`                  | Copy and paste selected nodes (without maintaining connections to outputs of unselected nodes)                     |
| `Ctrl` + `C`/`Ctrl` + `Shift` + `V`          | Copy and paste selected nodes (maintaining connections from outputs of unselected nodes to inputs of pasted nodes) |
| `Shift` + `Drag`                       | Move multiple selected nodes at the same time                                                                      |
| `Ctrl` + `D`                           | Load default graph                                                                                                 |
| `Alt` + `+`                          | Canvas Zoom in                                                                                                     |
| `Alt` + `-`                          | Canvas Zoom out                                                                                                    |
| `Ctrl` + `Shift` + LMB + Vertical drag | Canvas Zoom in/out                                                                                                 |
| `P`                                  | Pin/Unpin selected nodes                                                                                           |
| `Ctrl` + `G`                           | Group selected nodes                                                                                               |
| `Q`                                 | Toggle visibility of the queue                                                                                     |
| `H`                                  | Toggle visibility of history                                                                                       |
| `R`                                  | Refresh graph                                                                                                      |
| `F`                                  | Show/Hide menu                                                                                                      |
| `.`                                  | Fit view to selection (Whole graph when nothing is selected)                                                        |
| Double-Click LMB                   | Open node quick search palette                                                                                     |
| `Shift` + Drag                       | Move multiple wires at once                                                                                        |
| `Ctrl` + `Alt` + LMB                   | Disconnect all wires from clicked slot                                                                             |

`Ctrl` can also be replaced with `Cmd` instead for macOS users

# Installing

## Windows Portable

There is a portable standalone build for Windows that should work for running on Nvidia GPUs or for running on your CPU only on the [releases page](https://github.com/hanzoai/studio/releases).

### [Direct link to download](https://github.com/hanzoai/studio/releases/latest/download/HanzoStudio_windows_portable_nvidia.7z)

Simply download, extract with [7-Zip](https://7-zip.org) or with the windows explorer on recent windows versions and run. For smaller models you normally only need to put the checkpoints (the huge ckpt/safetensors files) in: Hanzo Studio\models\checkpoints but many of the larger models have multiple files. Make sure to follow the instructions to know which subfolder to put them in Hanzo Studio\models\

If you have trouble extracting it, right click the file -> properties -> unblock

Update your Nvidia drivers if it doesn't start.

#### Alternative Downloads:

[Experimental portable for AMD GPUs](https://github.com/hanzoai/studio/releases/latest/download/HanzoStudio_windows_portable_amd.7z)

[Portable with pytorch cuda 12.8 and python 3.12](https://github.com/hanzoai/studio/releases/latest/download/HanzoStudio_windows_portable_nvidia_cu128.7z).

[Portable with pytorch cuda 12.6 and python 3.12](https://github.com/hanzoai/studio/releases/latest/download/HanzoStudio_windows_portable_nvidia_cu126.7z) (Supports Nvidia 10 series and older GPUs).

#### How do I share models between another UI and Hanzo Studio?

See the [Config file](extra_model_paths.yaml.example) to set the search paths for models. In the standalone windows build you can find this file in the Hanzo Studio directory. Rename this file to extra_model_paths.yaml and edit it with your favorite text editor.


## [hanzo-cli](https://docs.hanzo.ai/hanzo-cli/getting-started)

You can install and start Hanzo Studio using hanzo-cli:
```bash
pip install hanzo-cli
comfy install
```

## Manual Install (Windows, Linux)

Python 3.14 works but you may encounter issues with the torch compile node. The free threaded variant is still missing some dependencies.

Python 3.13 is very well supported. If you have trouble with some custom node dependencies on 3.13 you can try 3.12

torch 2.4 and above is supported but some features might only work on newer versions. We generally recommend using the latest major version of pytorch unless it is less than 2 weeks old.

### Instructions:

Git clone this repo.

Put your SD checkpoints (the huge ckpt/safetensors files) in: models/checkpoints

Put your VAE in: models/vae


### AMD GPUs (Linux)

AMD users can install rocm and pytorch with pip if you don't have it already installed, this is the command to install the stable version:

```pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm6.4```

This is the command to install the nightly with ROCm 7.0 which might have some performance improvements:

```pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/whl/nightly/rocm7.1```


### AMD GPUs (Experimental: Windows and Linux), RDNA 3, 3.5 and 4 only.

These have less hardware support than the builds above but they work on windows. You also need to install the pytorch version specific to your hardware.

RDNA 3 (RX 7000 series):

```pip install --pre torch torchvision torchaudio --index-url https://rocm.nightlies.amd.com/v2/gfx110X-dgpu/```

RDNA 3.5 (Strix halo/Ryzen AI Max+ 365):

```pip install --pre torch torchvision torchaudio --index-url https://rocm.nightlies.amd.com/v2/gfx1151/```

RDNA 4 (RX 9000 series):

```pip install --pre torch torchvision torchaudio --index-url https://rocm.nightlies.amd.com/v2/gfx120X-all/```

### Intel GPUs (Windows and Linux)

Intel Arc GPU users can install native PyTorch with torch.xpu support using pip. More information can be found [here](https://pytorch.org/docs/main/notes/get_start_xpu.html)

1. To install PyTorch xpu, use the following command:

```pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/xpu```

This is the command to install the Pytorch xpu nightly which might have some performance improvements:

```pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/whl/nightly/xpu```

### NVIDIA

Nvidia users should install stable pytorch using this command:

```pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu130```

This is the command to install pytorch nightly instead which might have performance improvements.

```pip install --pre torch torchvision torchaudio --index-url https://download.pytorch.org/whl/nightly/cu130```

#### Troubleshooting

If you get the "Torch not compiled with CUDA enabled" error, uninstall torch with:

```pip uninstall torch```

And install it again with the command above.

### Dependencies

Install the dependencies by opening your terminal inside the Hanzo Studio folder and:

```pip install -r requirements.txt```

After this you should have everything installed and can proceed to running Hanzo Studio.

### Others:

#### Apple Mac silicon

You can install Hanzo Studio in Apple Mac silicon (M1 or M2) with any recent macOS version.

1. Install pytorch nightly. For instructions, read the [Accelerated PyTorch training on Mac](https://developer.apple.com/metal/pytorch/) Apple Developer guide (make sure to install the latest pytorch nightly).
1. Follow the [Hanzo Studio manual installation](#manual-install-windows-linux) instructions for Windows and Linux.
1. Install the Hanzo Studio [dependencies](#dependencies). If you have another Stable Diffusion UI [you might be able to reuse the dependencies](#i-already-have-another-ui-for-stable-diffusion-installed-do-i-really-have-to-install-all-of-these-dependencies).
1. Launch Hanzo Studio by running `python main.py`

> **Note**: Remember to add your models, VAE, LoRAs etc. to the corresponding Comfy folders, as discussed in [Hanzo Studio manual installation](#manual-install-windows-linux).

#### Ascend NPUs

For models compatible with Ascend Extension for PyTorch (torch_npu). To get started, ensure your environment meets the prerequisites outlined on the [installation](https://ascend.github.io/docs/sources/ascend/quick_install.html) page. Here's a step-by-step guide tailored to your platform and installation method:

1. Begin by installing the recommended or newer kernel version for Linux as specified in the Installation page of torch-npu, if necessary.
2. Proceed with the installation of Ascend Basekit, which includes the driver, firmware, and CANN, following the instructions provided for your specific platform.
3. Next, install the necessary packages for torch-npu by adhering to the platform-specific instructions on the [Installation](https://ascend.github.io/docs/sources/pytorch/install.html#pytorch) page.
4. Finally, adhere to the [Hanzo Studio manual installation](#manual-install-windows-linux) guide for Linux. Once all components are installed, you can run Hanzo Studio as described earlier.

#### Cambricon MLUs

For models compatible with Cambricon Extension for PyTorch (torch_mlu). Here's a step-by-step guide tailored to your platform and installation method:

1. Install the Cambricon CNToolkit by adhering to the platform-specific instructions on the [Installation](https://www.cambricon.com/docs/sdk_1.15.0/cntoolkit_3.7.2/cntoolkit_install_3.7.2/index.html)
2. Next, install the PyTorch(torch_mlu) following the instructions on the [Installation](https://www.cambricon.com/docs/sdk_1.15.0/cambricon_pytorch_1.17.0/user_guide_1.9/index.html)
3. Launch Hanzo Studio by running `python main.py`

#### Iluvatar Corex

For models compatible with Iluvatar Extension for PyTorch. Here's a step-by-step guide tailored to your platform and installation method:

1. Install the Iluvatar Corex Toolkit by adhering to the platform-specific instructions on the [Installation](https://support.iluvatar.com/#/DocumentCentre?id=1&nameCenter=2&productId=520117912052801536)
2. Launch Hanzo Studio by running `python main.py`


## [Hanzo Manager](https://github.com/hanzoui/studio-Manager/tree/manager-v4)

**Hanzo Manager** is an extension that allows you to easily install, update, and manage custom nodes for Hanzo Studio.

### Setup

1. Install the manager dependencies:
   ```bash
   pip install -r manager_requirements.txt
   ```

2. Enable the manager with the `--enable-manager` flag when running Hanzo Studio:
   ```bash
   python main.py --enable-manager
   ```

### Command Line Options

| Flag | Description |
|------|-------------|
| `--enable-manager` | Enable Hanzo Manager |
| `--enable-manager-legacy-ui` | Use the legacy manager UI instead of the new UI (requires `--enable-manager`) |
| `--disable-manager-ui` | Disable the manager UI and endpoints while keeping background features like security checks and scheduled installation completion (requires `--enable-manager`) |


# Running

```python main.py```

### For AMD cards not officially supported by ROCm

Try running it with this command if you have issues:

For 6700, 6600 and maybe other RDNA2 or older: ```HSA_OVERRIDE_GFX_VERSION=10.3.0 python main.py```

For AMD 7600 and maybe other RDNA3 cards: ```HSA_OVERRIDE_GFX_VERSION=11.0.0 python main.py```

### AMD ROCm Tips

You can enable experimental memory efficient attention on recent pytorch in Hanzo Studio on some AMD GPUs using this command, it should already be enabled by default on RDNA3. If this improves speed for you on latest pytorch on your GPU please report it so that I can enable it by default.

```TORCH_ROCM_AOTRITON_ENABLE_EXPERIMENTAL=1 python main.py --use-pytorch-cross-attention```

You can also try setting this env variable `PYTORCH_TUNABLEOP_ENABLED=1` which might speed things up at the cost of a very slow initial run.

# Notes

Only parts of the graph that have an output with all the correct inputs will be executed.

Only parts of the graph that change from each execution to the next will be executed, if you submit the same graph twice only the first will be executed. If you change the last part of the graph only the part you changed and the part that depends on it will be executed.

Dragging a generated png on the webpage or loading one will give you the full workflow including seeds that were used to create it.

You can use () to change emphasis of a word or phrase like: (good code:1.2) or (bad code:0.8). The default emphasis for () is 1.1. To use () characters in your actual prompt escape them like \\( or \\).

You can use {day|night}, for wildcard/dynamic prompts. With this syntax "{wild|card|test}" will be randomly replaced by either "wild", "card" or "test" by the frontend every time you queue the prompt. To use {} characters in your actual prompt escape them like: \\{ or \\}.

Dynamic prompts also support C-style comments, like `// comment` or `/* comment */`.

To use a textual inversion concepts/embeddings in a text prompt put them in the models/embeddings directory and use them in the CLIPTextEncode node like this (you can omit the .pt extension):

```embedding:embedding_filename.pt```


## How to show high-quality previews?

Use ```--preview-method auto``` to enable previews.

The default installation includes a fast latent preview method that's low-resolution. To enable higher-quality previews with [TAESD](https://github.com/madebyollin/taesd), download the [taesd_decoder.pth, taesdxl_decoder.pth, taesd3_decoder.pth and taef1_decoder.pth](https://github.com/madebyollin/taesd/) and place them in the `models/vae_approx` folder. Once they're installed, restart Hanzo Studio and launch it with `--preview-method taesd` to enable high-quality previews.

## How to use TLS/SSL?
Generate a self-signed certificate (not appropriate for shared/production use) and key by running the command: `openssl req -x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -sha256 -days 3650 -nodes -subj "/C=XX/ST=StateName/L=CityName/O=CompanyName/OU=CompanySectionName/CN=CommonNameOrHostname"`

Use `--tls-keyfile key.pem --tls-certfile cert.pem` to enable TLS/SSL, the app will now be accessible with `https://...` instead of `http://...`.

> Note: Windows users can use [alexisrolland/docker-openssl](https://github.com/alexisrolland/docker-openssl) or one of the [3rd party binary distributions](https://wiki.openssl.org/index.php/Binaries) to run the command example above.
<br/><br/>If you use a container, note that the volume mount `-v` can be a relative path so `... -v ".\:/openssl-certs" ...` would create the key & cert files in the current directory of your command prompt or powershell terminal.

## Support and dev channel

[Discord](https://hanzo.ai/discord): Try the #help or #feedback channels.

[Matrix space: #hanzo_studio_space:matrix.org](https://app.element.io/#/room/%23hanzo_studio_space%3Amatrix.org) (it's like discord but open source).

See also: [https://hanzo.ai/](https://hanzo.ai/)

## Frontend Development

As of August 15, 2024, we have transitioned to a new frontend, which is now hosted in a separate repository: [Hanzo Frontend](https://github.com/hanzoui/studio_frontend). This repository now hosts the compiled JS (from TS/Vue) under the `web/` directory.

### Reporting Issues and Requesting Features

For any bugs, issues, or feature requests related to the frontend, please use the [Hanzo Frontend repository](https://github.com/hanzoui/studio_frontend). This will help us manage and address frontend-specific concerns more efficiently.

### Using the Latest Frontend

The new frontend is now the default for Hanzo Studio. However, please note:

1. The frontend in the main Hanzo Studio repository is updated fortnightly.
2. Daily releases are available in the separate frontend repository.

To use the most up-to-date frontend version:

1. For the latest daily release, launch Hanzo Studio with this command line argument:

   ```
   --front-end-version hanzoui/studio_frontend@latest
   ```

2. For a specific version, replace `latest` with the desired version number:

   ```
   --front-end-version hanzoui/studio_frontend@1.2.2
   ```

This approach allows you to easily switch between the stable fortnightly release and the cutting-edge daily updates, or even specific versions for testing purposes.

### Accessing the Legacy Frontend

If you need to use the legacy frontend for any reason, you can access it using the following command line argument:

```
--front-end-version hanzoui/studio_legacy_frontend@latest
```

This will use a snapshot of the legacy frontend preserved in the [Hanzo Studio Legacy Frontend repository](https://github.com/hanzoui/studio_legacy_frontend).

# QA

### Which GPU should I buy for this?

[See this page for some recommendations](https://github.com/hanzoai/studio/wiki/Which-GPU-should-I-buy-for-Hanzo Studio)
