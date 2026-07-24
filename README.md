# 🚀 ONNX Image Upscaler — Complete Pipeline for Everyone

**Author:** [Jym Nils Caballero]
**Contact:** [[GitHub](https://github.com/jymnils2) /jymnils@gmail.com]

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jymnils2/upscaler-colab/blob/main/notebook.ipynb)
[![Abrir en Colab](https://img.shields.io/badge/Colab-Abrir%20en%20Colab-0277bd?style=for-the-badge&logo=googlecolab&logoColor=orange)](https://colab.research.google.com/github/jymnils2/upscaler-colab/blob/main/notebookesp.ipynb)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

## The Reality

Image super-resolution has advanced enormously. Models capable of upscaling images to impressive resolutions are published every day. But most users don't have a powerful GPU in their computer. This creates a gap: repositories full of extraordinary models that only those with dedicated hardware can use. If you don't have a GPU, you're left out.

Sound familiar? It did to me too. That's why I built this.

## The Solution

This notebook runs in the cloud. Google Colab gives you a free T4 GPU and this notebook does the rest. You don't need to install anything, you don't need special hardware, you don't need to know how to code. You only need a browser.

- **Windows PC** → works.
- **Mac** → works.
- **Chromebook** → works.
- **Android phone** → works.
- **iPhone** → works.

If you have a browser, you have a GPU.

## What's Included

This isn't a basic notebook. It's a professional pipeline with everything you need:

| Section | What it does |
|---|---|
| **Inference** | Upscales images with smart GPU tiling for any resolution. Downloads in PNG and JPG with embedded metadata. |
| **Conversion** | Transforms PyTorch models to ONNX with one click. Automatic architecture detection via Spandrel. fp32/fp16 precision selection. |
| **Models** | Complete model info card with OpenModelDB data. Editable personal comments to organize your collection. Safe deletion. |
| **Drive** | Persistent storage on Google Drive. Your models, info cards, and comments survive Colab session closures. Automatic sync between sessions. |

## Technical Features

- Tile processing with overlap to prevent seam artifacts
- PyTorch → ONNX conversion with dynamic axes for full tiling compatibility
- OpenModelDB scraping to generate model cards with architecture, scale, dataset, license, and author info
- Embedded metadata in ONNX files and in PNG/JPG output files
- Overwrite protection with auto-rename
- Professional web interface with 3 tabs (Gradio 6)

## Key Dependencies

Gradio 6 · ONNX Runtime GPU · PyTorch 2.11 · Spandrel · BeautifulSoup4 · Google Drive API

## Credits

- [ChaiNNer](https://github.com/chaiNNer-org/chaiNNer) — Inference pipeline inspiration
- [OpenModelDB](https://openmodeldb.info/) — Super-resolution model database
- [Spandrel](https://github.com/chaiNNer-org/spandrel) — Automatic architecture detection
- [ONNX Runtime](https://onnxruntime.ai/) — GPU-enabled inference engine

## Third-Party Licenses

This project uses the following open-source libraries:

| Library | License | Copyright |
|---|---|---|
| [Gradio](https://github.com/gradio-app/gradio) | Apache 2.0 | Copyright (c) 2022 Gradio, Inc. |
| [ONNX Runtime](https://github.com/microsoft/onnxruntime) | MIT | Copyright (c) Microsoft Corporation |
| [PyTorch](https://github.com/pytorch/pytorch) | BSD-style | Copyright (c) 2016-2025 Facebook, Inc. |
| [TorchVision](https://github.com/pytorch/vision) | BSD-style | Copyright (c) 2016-2025 Facebook, Inc. |
| [Spandrel](https://github.com/chaiNNer-org/spandrel) | MIT | Copyright (c) chaiNNer-org |
| [Beautiful Soup 4](https://github.com/wention/BeautifulSoup4) | MIT | Copyright (c) 2004-2025 Leonard Richardson |
| [Requests](https://github.com/psf/requests) | Apache 2.0 | Copyright (c) 2019 Kenneth Reitz |
| [ONNX](https://github.com/onnx/onnx) | Apache 2.0 | Copyright (c) ONNX Project Contributors |
| [NumPy](https://github.com/numpy/numpy) | BSD 3-Clause | Copyright (c) 2005-2025 NumPy Developers |
| [Pillow](https://github.com/python-pillow/Pillow) | HPND | Copyright (c) 1997-2025 Alex Clark and contributors |
| [onnxconverter-common](https://github.com/microsoft/onnxconverter-common) | MIT | Copyright (c) Microsoft Corporation |
| [onnxscript](https://github.com/microsoft/onnxscript) | Apache 2.0 | Copyright (c) Microsoft Corporation |

See [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md) for full license texts.

## License

This project is licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/).

**You are free to:**
- **Share** — copy and redistribute the material in any medium or format
- **Adapt** — remix, transform, and build upon the material

**Under the following terms:**
- **Attribution** — You must give appropriate credit and indicate if changes were made
- **NonCommercial** — You may not use the material for commercial purposes without explicit permission from the author

For commercial use inquiries, contact: [jymnils@gmail.com]
