# 🚀 Escalador de Imágenes ONNX — Pipeline Completo para Todos

**Autor:** [Jym Nils Caballero]
**Contacto:** [[GitHub](https://github.com/jymnils2) / jymnils@gmail.com]

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jymnils2/upscaler-colab/blob/main/notebook.ipynb)
[![Abrir en Colab](https://img.shields.io/badge/Colab-Abrir%20en%20Colab-0277bd?style=for-the-badge&logo=googlecolab&logoColor=orange)](https://colab.research.google.com/github/jymnils2/upscaler-colab/blob/main/notebookesp.ipynb)
[![Licencia: CC BY-NC 4.0](https://img.shields.io/badge/Licencia-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

## La Realidad

La superresolución de imágenes ha avanzado enormemente. Modelos capaces de escalar imágenes a resoluciones impresionantes se publican cada día. Pero la mayoría de usuarios no tiene una GPU potente en su computadora. Esto crea una brecha: repositorios llenos de modelos extraordinarios que solo pueden usar quienes tienen hardware dedicado. Si no tienes una GPU, te quedas fuera.

¿Te suena familiar? A mí también. Por eso hice esto.

## La Solución

Este cuaderno funciona en la nube. Google Colab te da una GPU T4 gratis y el cuaderno hace el resto. No necesitas instalar nada, no necesitas hardware especial, no necesitas saber programar. Solo necesitas un navegador.

- **PC con Windows** → funciona.
- **Mac** → funciona.
- **Chromebook** → funciona.
- **Teléfono Android** → funciona.
- **iPhone** → funciona.

Si tienes navegador, tienes GPU.

## Qué Incluye

Este no es un cuaderno básico. Es un pipeline profesional con todo lo que necesitas:

| Sección | Qué hace |
|---|---|
| **Inferencia** | Escala imágenes con tiling GPU inteligente para cualquier resolución. Descarga en PNG y JPG con metadatos embebidos. |
| **Conversión** | Transforma modelos PyTorch a ONNX con un click. Detección automática de arquitectura mediante Spandrel. Selección de precisión fp32/fp16. |
| **Modelos** | Ficha completa de cada modelo con información de OpenModelDB. Comentarios personales editables para organizar tu colección. Borrado seguro. |
| **Drive** | Almacenamiento persistente en Google Drive. Tus modelos, fichas y comentarios sobreviven al cierre de Colab. Sincronización automática entre sesiones. |

## Características Técnicas

- Procesamiento por tiles con overlap para evitar artefactos en las uniones
- Conversión PyTorch → ONNX con ejes dinámicos para compatibilidad total con tiling
- Scraping de OpenModelDB para generar fichas con arquitectura, escala, dataset, licencia y autor
- Metadatos embebidos en los archivos ONNX y en los archivos de salida PNG/JPG
- Protección contra sobreescritura con auto-rename
- Interfaz web profesional con 3 tabs (Gradio 6)

## Dependencias Clave

Gradio 6 · ONNX Runtime GPU · PyTorch 2.11 · Spandrel · BeautifulSoup4 · Google Drive API

## Créditos

- [ChaiNNer](https://github.com/chaiNNer-org/chaiNNer) — Inspiración del pipeline de inferencia
- [OpenModelDB](https://openmodeldb.info/) — Base de datos de modelos de superresolución
- [Spandrel](https://github.com/chaiNNer-org/spandrel) — Detección automática de arquitecturas
- [ONNX Runtime](https://onnxruntime.ai/) — Motor de inferencia con soporte GPU

## Licencias de Terceros

Este proyecto utiliza las siguientes bibliotecas de código abierto:

| Biblioteca | Licencia | Copyright |
|---|---|---|
| [Gradio](https://github.com/gradio-app/gradio) | Apache 2.0 | Copyright (c) 2022 Gradio, Inc. |
| [ONNX Runtime](https://github.com/microsoft/onnxruntime) | MIT | Copyright (c) Microsoft Corporation |
| [PyTorch](https://github.com/pytorch/pytorch) | BSD-style | Copyright (c) 2016-2025 Facebook, Inc. |
| [TorchVision](https://github.com/pytorch/vision) | BSD-style | Copyright (c) 2016-2025 Facebook, Inc. |
| [Spandrel](https://github.com/chaiNNer-org/spandrel) | MIT | Copyright (c) chaiNNer-org |
| [Beautiful Soup 4](https://github.com/wention/BeautifulSoup4) | MIT | Copyright (c) 2004-2025 Leonard Richardson |
| [Requests](https://github.com/psf/requests) | Apache 2.0 | Copyright (c) 2019 Kenneth Reitz |
| [ONNX](https://github.com/onnx/onnx) | Apache 2.0 | Copyright (c) Colaboradores del Proyecto ONNX |
| [NumPy](https://github.com/numpy/numpy) | BSD 3-Clause | Copyright (c) 2005-2025 Desarrolladores de NumPy |
| [Pillow](https://github.com/python-pillow/Pillow) | HPND | Copyright (c) 1997-2025 Alex Clark y colaboradores |
| [onnxconverter-common](https://github.com/microsoft/onnxconverter-common) | MIT | Copyright (c) Microsoft Corporation |
| [onnxscript](https://github.com/microsoft/onnxscript) | Apache 2.0 | Copyright (c) Microsoft Corporation |

Consulta [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md) para los textos completos de las licencias.

## Licencia

Este proyecto está licenciado bajo [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/).

**Puedes libremente:**
- **Compartir** — copiar y redistribuir el material en cualquier medio o formato
- **Adaptar** — remezclar, transformar y construir sobre el material

**Bajo los siguientes términos:**
- **Atribución** — Debes dar crédito apropiado e indicar si se realizaron cambios
- **NoComercial** — No puedes usar el material para fines comerciales sin permiso explícito del autor

Para consultas de uso comercial, contactar: [jymnils@gmail.com]
